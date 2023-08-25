# MVC


Inside our appstate is where we are going to store our arrays. (localStorage)
we build models to set up the classes for data to
we build controllers for each instance of data manipulation for the app.
We will also have a view that displays all the information in an organized way and allows us to manipulate it.
We will also have a view that displays all the information in an organized way, and interacts with user input.
We will also use a router to direct user input and display output.
Create an array in your local storage that you can access from anywhere within your application.
This way, when you refresh or close out of your browser window all of those items still exist on page load!
models files are used as a template that we can manipulate data from the appState with. 
controllers file are responsible for manipulating the model's data.
router file is used to route between different pages/routes.
Fist we make a model with "export class clssName{ constuctor(){}}"
Then we create a controller with "export default function(app){}"
Lastly we add routes to our AppState.js file with "import {route} from './controller'"
Now we have everything setup so lets start adding some functionality into our project:
Next we make a Controller in the controller file.
This is what handles the logic behind our views. We'll be using this to handle any event listeners that need to happen. 
We want this to be able to take in any parameters passed through it. This allows us to pass information about what action was taken by the user.
We need this because it allows us to call functions inside of our views.
after setting up the controller. we need to connect it to the router.
inside the router,js file is where we can connect our controllers and our view html/.
using switch we can set certain css classes that pertain to a specific set of data being brought it  form our appstate.
AppState.on is an example of an eventListener.
It listens for certain events to occur then runs code based off what happens.

## User Story: I want my todo list to persist even if I leave and come back to it later.
- [x] create a new class called TodoList
which extends from Model
- [ ] add a property to this class called todos which holds onto any tasks that have been added by the user so far
- [ ] add properties to this class like name, id, description etc...
- [ ] make sure these properties have getters and setters so they can be accessed outside of the constructor function.








## GregsList

to make a new page in your app go to the router and make a new path.
then import the component you created in the index.js file.
we can declare functions outside of the controller to make it a private function.
this makes sure they dont get exposed to other parts of the program.

## Thursday
