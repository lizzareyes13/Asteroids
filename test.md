1. What are three things you can do in order to speed up a website's load time? (Enumere tres cosas que se pueden hacer para aumentarle la velocidad a una pagina web) (20pts)

        answer: 1. place the css code at the top of the page in the header.
                place the JavaScript code at the bottom of the page before the
                ending of the body.
                2. optimize/resize your images.
                3. minify your html, css and javascript codes.

2. Go to the Google PageSpeed insights page and analyze www.carnival.com Choose three of the shortcomings this website has and explain the specific tools and workflows we discussed in class which could help this website address these shortcomings. (Dirijase a la herramienta Google PageSpeed Insights y analice el sitio www.carnival.com. Basado en lo que dice la herramienta, enumere tres medidas especificas que discutimos en clase para corregir tres de los problemas senalados por la herramienta PageSpeed Insights)(20pts)

          answer: the three shortcomings this website has are problems with browser caching, images need to be optimized and the website's codes need to be compressed.

3. Clone the repository named "Asteroids" from www.github.com/fvitech. Once you do this, complete the following steps:

        i. Fork the github repo so you have your own fork (5pts)

        ii. Clone your fork of the Asteroids repository (5pts)

        iii. Re-organize the files so image files are inside an img folder and js files are inside a js folder. (5pt)

        iv. Initialize your local version of the project as a node project (5pts)

        <!-- v. Install browserify, watchify, and all the required transforms so that you can have a single code bundle output to a file named prod.js (ES6 to ES5 conversion not required) (10pts) -->

        vi. The code is a bit messy, with many things in the same file. Modularize it by doing the following:
              a. Start by copying the contents of the codingIsFun.js file to a new file called main.js

              b. Create a watchify npm script to bundle your js code and create prod.js.(10pts)

              c. The Asteroids initialization code (which is marked by the comment which says GENERATE ASTEROIDS IN HTML DOCUMENT) should be in a separate file named createAsteroids.js. You will need to wrap this code in a function, export the function, then import this function and call it from main.js (10pts)

              d. The auxiliary functions keyDown and keyUp should be moved to a separate file named controls.js.

              e. The binding of the keyDown and keyUp events is currently being done in an attribute to the body tag. Change this by using JavaScript's document.addEventListener function.

              f. Your controls.js file should export a single function that configures the controls when called. Import and call this function from your main.js file. (10pts)

              g. No more than one script link is allowed in the main index.html. The only script that should be linked from index.html is prod.js

              h. Use uglifyjs to minify the code (20 point bonus)

              i. Upload your code to fvi-grad.com under your username (10pts)


        vii. In the end, all your JavaScript code should be inside a file named prod.js, which was created by using browserify

        viii. Notice that whenever there is a collision, the audio is being loaded and played. This slows down performance. Modify the code so that it loads the audio only once, stores it as a global variable, and whenever there is a collision, you use this clobal variable to reset the audio's currentTime to zero and then play it. (20pts)
