# Vue
vue is a middle frame work between react and angulare.
with the way that view workd is that our controllers pretty much show themselves as  pages in the file folders
the pages in view is going to similar to the mvc view
view has your html and the controller and the css in one pages
the componetnts in view lets us make functions our componets that we can call on or linke to another component for reuse
instead of mounting views and controllers we mount pages componetnts
the app.vue is the window to your appllication.
the router view is where all the routs in the router are
in the app.vue is where you can hardcode things. example: the header or login 
veet is a compiler so it take all the front end code and compiles it into js
veet also aout uplaods changes
in vue framework uses reatives and reactive mean is constanstanly watch any changes being made to the code. the obbserver patter is no longer needed
computed is the equivient of appstate.on
in the appState there will always be a user an account,
user is what comes back from authO and account comes from the server 
a V-if is an if statement ex. v.if="appState.account"
we put a setup inside of our script tag and in the setup is where private functions go 
you can think of this as similar to when we write functions in the conroller class
and if you want to access a method or a variable from you template thos will be declared there
in our dev tools we have a option for vue and thats how we can debugg our view
to sting interpilulate in vue is {{}} onclick is @click anything that is on or at is now @
to make a new pages we got to the router and first add iur path naming the correct endPoint
the component is where we say what pages we are creating
next we go to the pages folder and create a new pages file
from there we load up our template and our script tags
in our li tage we have to make a router link the router link takes up to a vue loaction
in order to render a router link you teed to tell the router link where to go using the to:{name: 'pageName'}
a lifecycle hook is 
onMounted: says as soon as it is mounted i want something to happen, as soon as this pages loads go get my data
ex. onMounted(() => {
    function()
})
pages are the parent the components are the children, when i want to pass data from a parent component to a child wee do that using props
computed almost always go on pages and "parent components"
there is heirarchy to the vue template.
we make a prop on the child component, each prop is its own entinty, we declsre them on child components to be ready to take in data
to pass the data to the parent we do that through tthe use of binding
a router link is 
inside of our to object is where we can put our params like :id/
: is th bind syntax
the parameter refers to the param in the router.js file
we can make sure the router link is working right by looking in our vue dev tools and click on the object to see if the params we have given it are actually passing through
const route = useroute give you access to the path we already on
router is for navigating and route is a specific path
to accses a parameter we say req.params.NameOfTheParamRoute
as soon as this page loads i want you to go and fire off a request and get me that beautiful data
you dont nessisarily need a try catch in in the on mounted method
to grab an id you need to const Id = route.params.Id
we use props when we want to draw something to the page more than once
we need to put our ids in the app.vue not inside the template
we need to make sure to declare toogle in th type :''
reading backdrop usually means you arnt targetting the right Id
make sure to use # inside the modal itself when naming the id
we use slot to take place of an area that we want to reuse and replace with different info or forms
a slot is the place holder for what you want to inject into it
we even need to make a forms seperatly in a compponet to use ar reuse in deffernent functions/methods/pages
make sure we have a formDiv wrapping all the forms used
refs are reative objects 
we need to format an object in oreder to posrt to the server, a ref will serve as the placehoder object for storing all the daya in the server
we use v-model to bind the user and give a live update throught the console on what is being updated in server
the ref is what allows us to put the v-model ont he forms or areas we want to save or see persist throught the appstate
we need to send the editable.value to strip the proxy layer
hint(unshift make it so something will jumo to the top of the array)
we can use editable.value={} is the vue equivilant to form reset
for Ui if you are going to use a icon on a button you must have a title tag

---------------------------------------------------------//wednesday//----------------------------------------------------------------

get things with an api we want them to get to the page
a paginated response means you are getting 20 objects back from an api at a time
first thing todo when bringing in an api we need to create the const in our auxios file
inside of our axios we can put our qerery params
any query request that you want from an api you just need to look at there docs
inside of our params we put our api key and any set params found on th docs in the api you are pulling from
after getting the auxios set up we need to think about what other architecture the site might need
inside the pagevue is where will set up our request from the api for the page in the on mounted method in the setup function
so in the setup is where we will make the functions but to declare them we need to declare it in the onmount
use the payload in the dev tools to make sure all params have been met
and in the preview we can make the data brought back is also what we were expecting
after getting a service registered and getting our api logged to the console we then can start to make our model to render the api list to the pahe
check the url that come through api and make the url that are coming back are full urls
interpilation is'words ${words}' concatination is 'words' + words
pay attention to the resposnse you get back from the api and make sure that your are accessing the correct response from the correcy data
in vue to talk to the appstste we use compute to bring data from the appstate we use a computed
we can then go to our template and and double {{}} and dump the data to the page to make sure we are getting back an data at all and rendering it to the page
get comfortable with v-for
in vue we abstract our template to it own componet insted of a modal
to pass data into a template we need to use a prop
we put props int the component the we have the template we want to call on
we then can call the prop in the page that we want to see it 
using a prop you need to you dot notation to get to the data we specifically want to see
remember that : is the binding syntax
in the router is where we set up a new page then we can make a vuepage then we can make components for it as needed
onMount is the equivalent to appstate.on
the easiest way to set an background image in vue is int the style css
we can go to a div and set a style tag inside next to the class then we can style = "{backgroundImage: 'url({movie?.background})'}"
  you can put type:text for places you want to take in text
  we then  can wrap it up in a form si we can subit the event handler
  when we send up a query we need to format it for axois can read it properlly
  with computd we need use appstae. insted of this.
  

\\\\\\\\\\\\\\\\\\\\\\\thursday////////////////////////
how to link accounts in vue! important 
in the router we can set up account commands that will run our aut0 functions
it is called the beforEnter: authguad
we can also write a function that inside that beforEnter(to, from, next){}
these are called router hooks
a component hook is onMount
how to edit accounts
in the account page we can guarantee that no one that make it to this page is not logged in 
we can go to the account model to get different info from the creatorId that we are not currently bringing to the pages
if you are trying to drill into something usiing dot notation that is set to null you need to you an elvis operator ??????
remeber to use your styling dev tool more
use and look up v-ifs
try to keep your pages and your components be no more that 100 to 150 lines if its more you need to make abstract to componest
raw data dumps are a good way to see where you template is resting the pages.
editables are how we can eddit things in our account we put  our const editable(name) inside the setup function
the v-model is what we sre going to change......more info 
watcheffects are a vue reactivities it is similiar to a computed its gong to watch over something and if something changes
{...} is a spread opperator {google it!}
every form has the same thing, its going to have an editable a watcheffect and a return editable for submit
you cant use a button on form that is labeled on sumit unlsess you call the button type button and you want it to do something other then submit
const editable = ref({})
editable.value
.value is the info iside of the array
to launch a modal make sure you are linking ti the id
and also make sure t add a data bs target
when calling in the modal in the id make sure you use a #Id
if the page complety gives out and wont load that probably means there is a rouer path error so check the router.js path name and route





in the terminal we use the startervue template.




first thing when bringing up the home page clear out the guts serve up the client and check out whats there
next set up the auxios service for the api we want to grab our indexs from
next we go to the homepage and make a async function in the setup above the return
this is where we will start our first get.(api) request
we will await our service and then make our service page for the api info
we will bring in our api.get
then we will want to log that we are indeed getting the indexs from the api auxios route then run and check our dev tools console
once we get the info in the console we need to make a place in the appstate for the array to live
when we put something in our appState we can look at it in our vue dev tool to make sure the array is in being found in the appstate
net get a template setup for our data to go
but to get the info that lives in the appstate we make a computed(()appstate.arrayName) make sure to put this in the return
next go to the template and make a v-for()
next do a data dump to the page {{}}
we can mess in the app.vue but be carful you can mess up somethings so only do it if nesseseser


so how do we get to see more than 20 things at a time. so make a button that says previous
and a button that says next.
so the data should bring in a url that has the next 20 things in the array
so add a @click to the button
then go the return and make a async function for changing to list from the api so send this function to the service
next we need to make a place in the appstate to save our nextIndex and our previosIndex
next we can in the get funtion we can say appState.previosUrl= res.data.previous and do the same for the next
now we can tie this in to the button.
so go to the return and make a computed for the previos and the next functions
then we can pass that in to our buttons as a parameter in the called @click fucnction(parameter)
then we can write our service function
we can tie it in to the auxios onstance and say api.get()make sure to reference thursday night firsisde when reading these notes
after finishing the function in the service we can check to make sure our data is being switched
to change the value of null we need to add a propertie disabled to the button disabled=!previous url
















\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\questions for tutor sesions////////////////////////////////////////////
how to search an api on the pages
how to use props 
what with the elvis opperators everywhere
how do we bind : im just confused on what we are binding it to




\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\ full stack design //////////////////////////////////////////////////////


first we need to use the express vue for the new full stack
first thing you do when you open your vs code is go to the work place
next set up the env.js with the right info from the sandbox
next start client then start server one those are done go to local host
best way to make sure the front end is connected to the back end is to lodin on the homepage
(the account comes from the dataBase and the userInfo is the Auth0)
after all of making sure the auth0 is set up next we make a model
on the back end the model is a schema
make sure to set up all virtuals needed in th model and next move to making a controller
and remember that the path tho our schemas is in the bgContext thats where we put our mongoose model
after getting the dbContext set up we can set up our service with a skelaton setUp
and then set up our controller with a skeleton setUp
remember that in the conteoller we use a constuctor and supers
class{
  constructop(){
    super(path)
this.router
  }
}


so now there postman tests, a postman test makes a request than analizes the response to see if gunna fail
whats important about the test is 

make sure to set up the authorization in post man and get your bearer token so we can run postman under our loggIn
for postman and for testing puposes our first step is gong to be post
make sure to folloe the set files in order in the postmans test
dont mess with set body of the test
inside of the respne after you run the test you can see the test results these will be very helpfule
req.body.creatorId = req.creatorInfo makes sure that the person creating the album is the verified user
make sure in our service we have a populate in our creat function


\\\\\\\\\\\\\\\\\\\\\\\\\\\                             front end                           ///////////////////////

On the client side the first step after starting up the client is to get model, but if its already made for our server Schema we can basically copy it for our model
in our model we can creator = new profile(data.creator)
and then we can set up our profile in the account model
it seems like good practice if you made the server to just make all the models needd since you already know the schema models from the server Side
after getikng the models set up we can move on to service
after making a service move on to making a get request from the selected api
after making the get function we can make  omMounted and check to see if were are getting any data
its seems to be good practice as well is to st up the template in the homePage then move it to the componet after the layout looks right
mave sure to use your vBind correctly
after aking the path in the router make sure to wrap up what we want as a clickable to be wrapped in a router link
in the router link we need the name of the page and params with :id
once the router is set upmake sure the links are sending you to the right page
then we can work on drawing the data to the new page
in side the new page is where we start making our get functions
then get them in the onMounted and loaded to the screen 
to access the the router we need a const route = getRouteById
then we need to make sure we make our service side functions after the page is set up
we need to think about the data we are wanting or getting back and make services and component accordinly
we can reference paths/endpoints in the serverSide to mae sure we are hitting the right endpoint
the @type {import} its making sure that our models are being read right
when usin a model you need to add a slot <slot> </slot>
a slot is a placceholder,it is essentialy doc.getElementById
inside our form we can use the select tag for a list of things to choose and in that tag we can put an option tag with the options that we want
useRoute means it will navigate to one page, while useRouter gives us accesss to our whole vue.page
if you dont want to deal with elvis oppperators wrap your template in a v-if
remember to use a @submit.prevent to stop the page from rloading after the submission of the form
if we are trying to inject something into a modal to draw and somethings broken then it will affect the modal from opening
if you have a rule on the front end the server need to reflect tha rule


in the back we start our modes with a schema
in the collaborator schema shows how we are tying together an album to an account for reference
a virtual always has a foriegnfield, localField, ref, justOne.
make sure to register all the models inside of our dBContext
then we can make a controller
make suer that the base controler gets imported, inside the super ake sure that you hitting the correct endpoint
if we are psoting make sure to put a .use (authProvider)
then we can make our functions we req.body.accountId than it can be passed to the servvice as needed
make sure we are populating on the 
the account is ment for outorizing the account user


how to do a count on profiles following
look at the docs for the cirtuals on mongoose.
Befor maing code for the new checkPoint write out a good outline of what services, controllers and models that are needed
do the same for the front end befor you start coding
make sue that in postman we set up our baseUrl and our bearer token in the variables 
besure to make sure we are pasting all postman tests, however we get that
when we have multipule functions we need to have placehoder
you can write anonamos functions in the computed
make sure to reference how the did the filter on the front end with there buttons on the post-it app
tonight and tommorw let make sure all of the back end is done befor over to the front end
this checkpoin is going to be tricky so make sure that you focus hard o functionality
remember that our v-for is our for loop for looping over our array and draing the information that is desired
remeber using Vue that you need elvis oporators or a vIf over the whole desipred data template
we can nest computed ref post_it
our . Appstate.find gives reactivity



