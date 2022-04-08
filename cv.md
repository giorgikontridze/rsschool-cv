# **Giorgi Kontridze**

## **Contact Info**  

Location: Georgia, Tbilisi  
Mob: +995555775579  

[Email](mailto:giorgi.kontridze21@gmail.com) / [LinkedIn](https://www.linkedin.com/in/giorgi-kontridze-20515a184/) / [GitHub](https://github.com/giorgikontridze/)  

___
## **Summary** (your goal, wishes, reveal what is important for you, what do you want and why.
Some kind of self-presentation. In case of lack of experience  Junior Developer sells his/her potential, his/her passion and ability to learn fast. You shouldn't think that everybody is going to teach you when you come to the workplace . Rather being a Junior means always
learning new things from everywhere etc.).
___
## **Skills**  

* Git
* GitHub
* Markdown
* HTML
* CSS
* JavaScript
___

## **Code examples**  

<details><summary>Blinking rectangles</summary>
<p>

    ```js
    /*  This program devides the canvas into an imaginary grid with rectangles and
    *   changes rectangle color on user mouse move.
    */

    var NUM_RECTANGLES_ACROSS = 4;
    var NUM_RECTANGLES_DOWN = 10;
    var RECT_WIDTH = getWidth() / NUM_RECTANGLES_ACROSS;
    var RECT_HEIGHT = getHeight() / NUM_RECTANGLES_DOWN;
    var transparent = new Color(255, 255, 255, 0.6);
    var grid;
    var START_X = 0;
    var xPosition = START_X;
    var yPosition = getHeight() - RECT_HEIGHT;
    var element = null;

    function start() {
        setTimer(drawGrid, 1);
        mouseMoveMethod(blink);
    }

    //This function changes the color of rectangle on mouse move
    function blink(e){
        element = getElementAt(e.getX(), e.getY());
        if(element != null){
            element.setColor(Randomizer.nextColor());
        }
    }

    //This function draws grid with rectangles
    function drawGrid(){
        if(getWidth() - xPosition > 0){
            grid = new Rectangle(RECT_WIDTH, RECT_HEIGHT);
            grid.setPosition(xPosition, yPosition);
            grid.setColor(transparent);
            add(grid);
            xPosition = xPosition + RECT_WIDTH;
        }else if(yPosition > 0){
            xPosition = START_X;
            yPosition = yPosition - RECT_HEIGHT;
        }else{
            stopTimer();
        }
    }
    ```
</p>
</details>
 
___

## **Experience**  

### No work experience on a real project

### Projects from courses:  

* Brakeout on codeHs.com - [Run Breakout game](https://codehs.com/share/id/write-the-code-3EllXd/run)
___

## **Education**  

- CodeHs - Programming foundations
- Codecademy - Basics of HTML / CSS / JavaScript
- freeCodeCamp - Responsive Web Design (HTML / CSS)

## **Language**  

* Georgian: native
* English: B1
* Russian: B1
___