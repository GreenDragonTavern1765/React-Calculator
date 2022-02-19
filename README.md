# Calculator Web-Application in React (JavaScript Framework)
The purpose of this project is to practice and get familiar using React for an upcoming capstone project.
This is a basic calculator web-application on the React JavaScript framework, and is being developed using 
WebStorm, a JetBrains JavaScript IDE. Throughout the development of this web-application, activities will be
logged using this README.MD file as documentation for the process itself, and will be updated with each commit
to Github.com using the resources available from an online YouTube tutorial on the React environment.
The link to the video is https://www.youtube.com/watch?v=oiX-6Y2oGjI

### Initialization
Firstly, the project itself must be created, and some changes need to be done to make the project ready for
development, deleting a few initial files and removing invocations of those files within other files. For the
last part of this step, as always, make it a 'Hello World' banner to make it official.
1. Create the project, named 'React-Calculator' which is a React Project
2. Delete some initial files generated during project initialization, and make changes to others
   1. App.test (Delete)
   2. App.css (Delete)
   3. Logo.svg (Delete)
   4. ReportWebVitals.js (Delete)
   5. SetupTests.js (Delete)
   6. Index.js (Remove instance of ReportWebVitals)
   7. App.js (Remove import statements for Logo and App.css, and everything inside of App class)
3. Remove all contents from Index.css, will be added to later on
4. Finally, add the Hello World banner to the App class in App.js

### Development Part 1 (HTML setup)
This section is the HTML initialization of the project, creating the buttons that will be interacted with
by the user, as well as setting up the classes that will be manipulated using the css files in the project.
1. Type 'npm start' in WebStorm terminal, load up the React Development Server
2. Create 'calculator' class and a 'display' and 'operators' class within calculator
3. Create 4 buttons within the 'operators' class (+, -, *, /)
4. Create a 'Digits' class
5. Write function to generate digit buttons (1, 2, 3, 4, 5, 6, 7, 8, 9)
6. Invoke function within digits class

On the client side, this is what the project looks like so far, it lacks formatting that will be added in
as the development phase proceeds.
![img.png](img.png)

### Development Part 2 (CSS formatting)
This section will cover the CSS formatting, this will take the code written from part 1, the buttons, the classes
everything, and will format it and make it nice.
1. Created 4 css variables, used to designate certain colors used throughout formatting
2. Formatted the classes and centered them to make the calculator in the middle of the screen
3. Added background color and formatting to each of the types of buttons (classes)

On the client side, this is what the project looks like so far, it has the aesthetic look of a finished up,
all that is left now is to add the functionality to the calculator to let the buttons do something now
![img_1.png](img_1.png)

### Development Part 3 (App Functionality)
This section will cover the manipulation of the JavaScript code in App.js to add levels of functionality to
the app, making the buttons for the digits and operators actually do something.
1. Created multiple arrays for calculating and storing the results, as well as holding the char value for each operator
2. Wrote an arrow function called updateCalc which will update the calculations from before
3. For each button, added the updateCalc() function with the attribute of OnClick() which will added it when that button is clicked
4. If statement added to updateCalc() function, if an operator is clicked before values are put in, nothing happens
   1. If the last value that was input was an operator, then operators cannot be clicked again, preventing two operators from being in the same expression (++++, ----, +*/-)
5. Added calculate function to calculate the expression typed in by user
6. Added deleteLast function to delete the last value input by the user