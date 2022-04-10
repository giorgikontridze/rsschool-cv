# **Giorgi Kontridze**

## **Contact Info**  

Location: Georgia, Tbilisi  
Mob: +995555775579  

[Email](mailto:giorgi.kontridze21@gmail.com) / [LinkedIn](https://www.linkedin.com/in/giorgi-kontridze-20515a184/) / [GitHub](https://github.com/giorgikontridze/)  

___

## **Summary**  

At the present moment I am the head of the Geographic Information Systems group at the leading company of telecommunications field in Georgia. My main experience comes into contact with administering Windows, SQL, GIS servers. I’m qualified in document analysis and problem solving in this area. I have always been obsessed in programming and made decision to make an effort at this field. From my personal traits I distinguish purposefulness, the ability to do the job with due diligence and with best quality, and the capability to fulfill  the job at all events. My main target is to become a full stack developer, furthermore I'll do everything possible to achieve this goal. However I guess that working on a real project, is the best way to gain practical experience. I believe I’ll get a chance to express my skills, to obtain relevant knowledge and to become the member of your big family to support you in implementation of projects.

___

## **Skills**  

* Linux
* VS Code
* Git
* GitHub
* Markdown
* HTML
* CSS
* JavaScript  

___

## **Code Examples**  

<details><summary>Blinking rectangles (JS)</summary>
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

No real project experience

Projects from courses:  

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