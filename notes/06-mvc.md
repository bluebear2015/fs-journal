# MVC
application design patters
mvc design patterns 
mvc stands for THE MODEL THE VIEW AND THE CONTROLLER
mvc is there are a million mvc flaveors
veiw - html dom index.html. html representation of the data in the app
controller - takes in actions from the user draws data to the dom
service - business logic happens, anything that modifies data goes here
appstate - single source of the truth aka where all the apps's data will be stored
model - blueprint of what the data in the appstate looks like this is the deffinition of what data will be
the service is the meat and potatoes of the mvc model
the mvc model is scaleable for most any project
npm i -g bcw 
then bcw create than choose which project template you want then choose mvc
there is a pattern in place and we need to follow that pattern
new keywords: this(means this insstance this time around)
new lets you creat something brand new
import system links up files to the js
you have to export an element to be able to import it
the coontroller can see new data through an observer
onmousedown means click
te draw function is the thing that changes the page
subscribing to the changes in data: so that; i can draw when needed
a constuctor is resposible for building things it a special function instantiating a instance or a class
the constuctor needs to take in data or raw material
you can put the constructor inside of a class
in this constructor data represents a object
string is going to usually a word
order matter || can be used to say or in javascript 
all data is being stored in the app state
inside of a class you dont need to use let or var and you can put arrayName=[ for an empty array space]
make sure to export and import betwwen pages to get functions to work with function described on differnet code pages
make sure import into the app state and make sure to export first
look up SCOPE
you can call on other functions or arrays or object between different files by using fileName.ObjectName
classes have a constructor and when classes are invoked the constuctor inside of that class takes place
make sure you get the pathing correct 
you can make html adjustments right inside of the template whenre the template has been assigned
use back ticks to assign whats a 'string' and whats and object
this is called object oriented programming
it is never the job of the controler to modify data just because it shouldnt
singleton patterns means there is only one
export const heroservice = new heroService()
usually what tarts in side of a parmeter in the beggining is usually ended with that same parmeter at the end of an argumert
our services page is essinctialy what we want our page elements to do
the controllers job is to draw from the page
using appstate.emit('') will trigger listeners to fire essientially a for each loop
use figma more!
follow this same patern
-creating files first so make in the model
and you need to always create a new file inside of the model section
if we want to be sble to reference this class elswhere in our project make sure to add export
kind of think of the model class ass a blueprint like you would in css
think of the constructor(){} as the invoker inside of the class
 example the constuctor is waiting for an object to attach to
export class Classname{
    constuctor(walls, floors, windows){
        this.walls
        this.floors
        this.windows
    }

}
so if i wanted a new house 

newHouse({walls:'plywood','floors:'tile', windows: 'glass'})
-imports export

-then work the model

contollers; are the filter layer btween the users and the rest of the app

models:  is what i want my data to look like

services: are responsible for data(appstate) manipulation so 

appstate: where i want my data stored so this is where er would put our arrays when making a new array use new and name the class with({constuctor values})

app.js is essientially the window to the rest of our javascript

remeber that || means or so you can use || '' for or default
if we export with a const to export a single instance of a class for there single need
if you want something to happen as soon as the page loads we can throw it in the constuctor
consol.log from the controller to make sure it is hooked up properly
when we get to labs make you model, make your services, make your array in the appstate, then link up your controler
use get NameTemplate(){
    return` copy and paste the dive you want as the template
    inside of template you can use '${app.controllerName.function}'
}

anytime you make a draw function
to make something happen as soon as the page loads put it inside the constuctor
let name =appstate.Nme to call on a value inside another file
@type{import ('./models/gachamon')}
a pivate function needs to be denoted by an underscore
backticks allow you do string interpilation 
setHTML does the same thing as getDocumentByID with the first value being the div id
you want to put your template in the models
a function is delcared outsied of a class
when i declare a function inside of a class its called a method
when calling somthin in side the template make sure to use app. to access things in the app, because the app is the only thing linked to the html
html{ what is on the page
    app{ what info the user can see
        contollers{ data the user can manipulate
            services{
                models{

                }
            }
        }
    }
}
use command .
click onto i function hit command . to declare this in service
nameService = 
anytime you want to access the app state go thru the service layer
appstate.on('activateGachamon', drawActive)
make sure to register all controlers in the app.js
rember all data maniputlation is done all in the service
service is what manipulates the app state
if you have set ativie in the contolers you should have set active in the services
math.floor(math.random)
always use the appstate to save data and arrays
models is where me model the data for thw page
.push()will puch somethiing into an array
so in the app state if we have myArray = []
we can yse the .push to save something new to that array
myArray.foreach(g <= template += g.list template)
we can use manual emit to add a value to something?
with saveState(bannana word, )
myNAme = loadState(banana word, [arrayName])
load state is basicaly parcing the save data into the array
hold alt to place multiple cursors
labs
start with making a model array
the controller always manipulates the dom
when you are creating a constuctor for one single thing name it with singular casing as opposed to something like an array we use plurle casing
make sure to registure the controllers in the app.js because app.js is the file that actually gets control of the page
/look up scss/ it sounds like css combined with javascript
int the terminal run npm i to download node moduels
then run npm sass to chang default variables in sass
using getcars attached to a onclick then putting the draw function inside of it to get something to the page when clicked on the set onClick button
get is essentially additional properties and we can access them with .notation
remeber the controllers is specificaly for manipulating the dom
make sure the my place holder template is placed outside of the for each
setHTML means you are setting a whole block of html where as setText on sets text inside of a element
data bs toogle and data-bs-target
use modals and ask for help if needed
in the modal dialog class if where you can change
use get ActiveTemplate(){'copy and paste html section in here'} 
when using template rows are typically always its parrent container so make sure to template underneath the row div
services are not registered to the app, only the contolls do
appstate.on lets the current function to listen for any changes in the app state
mkae sure the label matches the id
you can put a min lenth and a max length on a form and putting required on it it will make it so you have to fill out a form to proceed at the type 
on a form you need to specify if its for text or for numbers
type is how you control the input so text numbers img or color
at ate top of the form write onsubmit then connect it to the controller
use windoe.event.preventdefault() to prevent the page from resetting
static vs get
get sets everytime the page loads
static
static carform
you can reuse forms are modals by using static
input value is what the user has put in to an input
key value pairs are name(key):nameOfObject(value)
the label tag is the label for the input
appstate.emit to push thing in the dom?
botstrap.modal.getorcreatinstance('#modal').hide() to hide modal when finished
we use static template for some thing that is there but doesnt nesseraly drawing any info from the appstate
anytime we want to save a changes to the appState in local storage use saveState('cars', appstate.cars)
industry best practice is use _() on any private function
(what collection you are trying to bring in or the key, )
import pop to make a nice looking log in
we go through the service wwhen we want to talk to the appstate
use if(!input) return to make 


very first create a model file formatting any of your properties takes place inside the model
make sure to import the model to the appstate
followed by export class with a constuctor
us || geratetID() to get random id


export class Name{
    constuctor(data)
    this.name = data.name
}

second thing after conecting the model to the appstate then create a controller then build a service

service export class CasesController {  }

export const casesController = new CasesController
then register the cases controller
test the controller by loging to the console in the constuctor of the controller
next set up your html for wher you want thing to go on the page
create p tags and h1 for each data property you want drawn to the page
start using stubs more
 with template
 inside the model constructor use
 get NameTemplate(){
    return`paste Template here`
 }

then we need to make a draw function
--------vvvvvvvTHESE ARE ALL INSIDE THE MODEL-------vvvvvv-------------------
let Name = appstate.Name
let template = `` 
name.foreach(n => Template += n.name.Template)

get computeDate(){
    let date = this.date
    return (date.getMonth()) + '/' + (date.getDate())
}
^^^^^^this puts month day year^^^^^^^^
get ComputeTitle(){     (goes vvv for specific info nside of a string)
    return (this.reportBody.slice(position in side the string)) + '....'
    let foundName  = appstate.Array.find(c=>c.id==cases) to 
}
textarea has a name attribute that corralates with what property you wan to selct
 we use appstate.on to listen to what activeity is happening in the page and act accordingly

 let methodName = this.reportBody.split(` `)
 ^^^^^^^^^takes the original report body and turn it into an array of individual words
 use .map iteratete items in an array to change certian things in it
 best way to flip a boolean is founcase.unlocked = !foundcase.unlocked
 use name.filter(n => n.)
 use saveState and loadState

 ----------------DEBUGGING--------------
 always link up your controller in the APP
 anytime the coonsole says reserved word that mean we are putting a word thats reserved for a different function
 look up asyc and


 ------------------Tueday weeek4---------------------------------

 sandbox.codeworksacademy.com
 jwt.io will give you your access token
 use mvc-auth for new template today
 when you enter the templat your gong to use the key provided by sandbox
 after putting in our key we can remove the card auth template
 we can use <a href="#about" class= "link"> direct to a differnet page
 we now have a ENV.js is a new file in the new template
 the ENV file is where we go to load up the enviorment for the application
 this is where wer put our 3 keys from the sandbox
 we also need to past the sandbox.com url in the base URL spot
 if done right our envirmoent card should be all plugged in on the page
 we then can login in the promt when page loads
 the beaer token is the user id
 after all this we can delete our template for the auth controller
 users are now full object not just a string or a name
 ROUTER
 inside of this we hace a path path is the direction you want to dirct the page
 we also use route to essenctially catch the path direction and ('_')
probably swith to bcw serve insted of live
biulding out craistlist
1. putting a page
use the Href#/cars
now cars controller setup
export class controller{
    constructor(){
        always console.log ('')
 
    }
}
 next we are going to register the car controller in the router
 if done right our console log should come up
 the router initialises the controller but for the specific page so if you go to the about page our console log should not come in
 next we need to make our car service  with our class cars and an export const carservice
 class carsService{
async getCarsFromApi(){
const res = await api.get('api/cars')

}
 }
then import the carsService to the cars controller

in side our our car controller we can make our asynce GetjobsFromApi(
    try{ awit.jobservice
        catch
    }
)

now we can go back to the cars service to get the data
we use .map but you always need something to  map over so we make our modal this the this.data
control to intelesence move to make changes to matching objects on a line for quick name changes
res.data.map(j => new jobs(c))
make a function so while the page is loading we log something to the page
we can se html in the constructor to show something while its being fetched
static jobform(){
paste modal or template
}
inside the cars controller you can ust setHtml(modal-guts, jobform())
inside of our button we can use data-bs-toggle= 'modal' data-bs-target='#modal" the target need to alwat match the id of what we are targetting
we can also put a buttn inside of a setHTML(buttonId',"") to load with the hidden button inside the home controller
if(appState.accoutn){
    setHtml(id name) to have to app listen to when someone is logged in to load our state
    anttime you use async you always need a try{
    } catch (error){pop.error(error)}
} 
widow.event.preventDefault() to prevent from refreshing the screen when a user action takes place
const formdata =window.event.target
const formdata = new formdata
to start our save form data function
log(to see the saved data)
the we need to cal on the service with an awiat carService.
next we need to make a new car formdata function in the service
async createjob(formdata)
now we need to send the formData to the server
cost respose = awiat api.post('api/cars', formData)
the service is what should be talking to the server
if the save was successful we should be able to log and see our formdata
it does depend on the api you are using how it will proccess that info
now if we can see the logges data
we save it by const newcar = new Car(res.data)
then we need to push it to the appstate

delete button on our modal form
onClick = app.carsController.delete job('dealetJob')
 
 asyc deleteJo(id)
 try{


 }catch(error)
 pop.error(error)

 connect this to the car service

 create a new async method
 async always id followed by awiat
 we can check our car deletion in the dev tools network tab
 get rewuest is a read request a post requste is a create
 put request is a update
 delete is delete