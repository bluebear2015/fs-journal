# Vue

vue is a frint end framwork that is "reactive".
Javscript is the core language.
HTML and CSS are used to build user interfaces.
Vue has its own templating syntax called `template`.
`template` can be written in HTML or JSX (a superset of JavaScript).
in your own time learn React and Angular front end frameWork.
we now are going to use the view starter template fro the terminal.
remember to reference the view docs.
we no longer use bcw-serve we now just spin up our client and then go to localHost 8080.
this will have hot model reloading which is reactive with the code and auto reloads the page anytime you mak a saved change in you vsCode.
things like the jsConfig and the EditorConfig. are all designed to tell the vs code that this is a vue project and to treat it appropriately.
our package.json holds our dependencies.
the vue cli will install these for us when we run npm i.
our source folder has all of the files that we use for our app as of now.
main.js is the entering point of our application.
our registerGlobalComponets.js looks at our components folder and automatically registers them.
all of what we would call controllers are now components.
components have their own data, methods & events.
data is stored on the component instance which means it's not shared with other instances.
methods allow you to perform actions within an event handler.
events let you listen out for certain things happening inside of your component.
you can also pass props into child components from parent components using the prop attribute.  
props are read only by default but you can make them mutable if needed.
encapsulation and abstraction are the main pillers of OPP that we are using with .vue for now.
this way we don't need to worry about how everything works internally.
V- is a vue attribute. 
@click is short hand for  V-bind: click.
if you have more than 150 lines of code you are writting to big of a file.
in the bottom of our components page is were we have our style tag for our custom css.
we dont have to make draw functions anymore in our view file is where we make our templates that will draw to each individual template through the .vue component.
if you get an error for callstack side exceeded it means you have a recursive component.
to fix this we should move some logic out of the render function so that it doesn't cause a stack overflow exception.
it needs to break down further so it doesn't exceed this limit.
inside the set up in our export default class is where we can declare methods and call on functions.
there a couple was to make a element reactive, ex. ref().
a double bind {{}} in vue ill take a whole object no matter what it is and display the whole manipulated object.
we can access the value of any variable using $refs.
when working with refs remember to add v-model="name" to input field.
v-for loops through items in array.
each item gets passed to looped Item.
to create a new object we do Object.assign({}, obj)
Object spread operator allows us to copy properties over without having to write each one individually.
computed property returns values based off of other variables.
watch() method watches for changes in specific variables.
emit sends messages back to the parent component.
parent refers to the immediate parent scope.
we need to put computed(() => AppState.name)
so it knows to watch for changes in the AppState and to render the data to the screen when changed.
:diabled = "parameter == parameter".
we access our AppState by using a computed(() => AppState.name)
we want to disable button until name is filled out correctly.
we can use :disabled=true or disabled=false.
we can also bind multiple parameters together like @click="method(paramOne, paramTwo)"
we can even chain methods together like @click="methodA(), methodB()"
we can also use keyup.enter to trigger a function.
we can also use v-once directive to prevent re rendering of elements.
we can use v-html directive to display html content.
we can use v-show directive to show/hide elements depending on conditionals.
we can use v-cloak directive to hide unrendered elements while they load.
we can use v-pre directive to preserve spaces and line breaks.
we can use v-text directive to change text content of DOM node.
we can use v-model directive to link two-way binding between form inputs and Vue model.
we can use v-slot directive to define named slots.
we can use v-slot:default slot to provide fallback content.
we can use v-slot:named slot to specify target container.
we can use v-on:keyup.enter="" to attach listener directly instead of writing full syntax.
we can use v-else directive to check against previous conditions.
we can use v-else-if directive to check against additional conditions.
we can use v-once directive to stop updating nodes after first update.
we can use v-memo directive to memoize expensive computations.
we can use v-is directive to dynamically switch markup structure at runtime.
we can use v-once directive to skip updates of child components.
we can use v-model directive to implement two-way bindings.
we can use v-model.number modifier to convert string into number type before setting value.
we can use v-model.lazy modifier to wait till user finishes typing then apply changes.
we can use v-model.trim modifier to trim whitespaces from start & end of strings.
we can use v-bind directive to pass dynamic attributes to HTML elements.
we can use v-bind:class directive to assign classes to HTML elements.
we can use v-bind:style directive to style HTML elements inline styles.
we can use v-bind:id directive to give unique identifiers to HTML elements.
we can use v-bind:ref directive to reference an HTML element inside template.
we can use v-bind:key directive to uniquely identify list items.
we can use v-bind:srcset directive to manage responsive images.
we can use v-bind:href directive to set links destination address.
we can use v-bind:download directive to download files automatically.
we can use v-bind:draggable directive to make elements draggable.
we can use v-bind:contenteditable directive to enable editing of innerHTML.
we can use v-bind:tabindex directive to control focus order with tab keys.
we can use v-bind:autofocus directive to autofocus input fields during page loading.
we can use v-bind:readonly directive to lock down input field so users cannot edit them.
we can use v-bind:required directive to mark required fields as such.
we can use v-bind:maxlength directive to limit character count within input fields.
we can use v-bind:minlength directive to enforce minimum characters requirement.
we can use v-bind:pattern directive to validate values based on regex pattern matching.
we can use v-bind:placeholder directive to add placeholder text to input fields.
we can use v-bind:accept directive to restrict file types allowed to be uploaded.
we can use v-bind:alt directive to describe image contents if image fails to load.
we can use v-bind:autocapitalize directive to capitalize the first letter in each word.
we can use v-bind:autocomplete directive to improve autocompletion for forms.
we can use v-bind:spellcheck directive to turn spell checking on / off globally.
we can use v-bind:translate directive to translate content using Google Translate API.
we can use v-for directive to loop through arrays or objects.
we can use v-for="(item, index) in array" to iterate over object properties too!
we can use v-for="n in 10" to create simple loops.
we can use v-for="user in users | filterBy searchText" to pipe data through filters.
we can use v-for="(value, key, index) in obj" to access all three indices simultaneously.
we can use v-for="(value, name, i) in {a:'foo', b:'bar'}" to destructure object properties.
we can use v-html directive to render raw html code.
we can use v-show directive to show/hide elements conditionally.
we can use v-cloak directive to hide unrendered vue instances until they are ready.
we can use v-pre directive to preserve whitespace when rendering templates.
we can use v-once directive to prevent reactivity and DOM patching.
we can use v-text directive to bind a piece of plain text.
we can use v-model directive to handle form inputs.
we can use v-slot directive to define named slots that we can later fill up.
we can use v-on directive to listen to native events like click etc..
we need to put our v-for on the thing we want repeated, so don't put it directly on the component itself.


# -------------------------------TUESDAY------------------------------------------
Today we will be using vue-starter template from the console.
Dont forget to npm i to bring in all dependencies for the .vue template.
first we start with a model bring in our data from the API.
Then from there we go on to make a service and a controller.
in .vue if you dont need to pass a value or parameter you dont need to have().
lifeCycle hooks are onMounted(), onUpdated(), onUnmounted().
all members inside of the return get read by the template.
In the axios service is where we are going to go register our API we can also add our params for what content we want to  bring in from the API.
We then can go to our service andd make sure that our API endPoint is correct
after Getting our data drawn to the console move to the AppState and give it a local place to live as well.
then from there we can map out the data that is being broght in.
Make sure to look at the data and see what the Array name is.
you cannot import a single item in an array we need to use props.
props are used to send information into components.
Props are passed downwards (child -> parent).
You can also pass props upward(parent-> child), but this should not be done unless necessary because it makes your app more difficult to maintain.
Props are immutable unless explicitly declared otherwise.
on our forms we need to put @submit for .vue
# Thursday
we start by loading the vue starter from the terminal.
make sure we put in our sandbox info is plugged with our information.
after the env file is set up we can then spin up the client and then go to localhost 8080.
ocne we have our localhost 8080 running we should log in so we can get our token and make sure auth0 is set up properly.
first thing we should do is go set up our model with the data that we are trying to pull.
then we can go ahead and build out our services and controllers.
we can also add some life cycle methods here such as mounted() which runs after the page has loaded, and we put this on the page we are working with.
from here we can begin building out our app state which is where we store everything.
Once we get the data to run to the console we then we should try to get it into our page.
we can go this by using our map function in the service layer.
this allows us to take the data coming back from the api call and turn them into something more usable within our application.
then to bring in our model from the service layer we need to add a computed in our return calling on the array stored in the appstate.
after getting our computed set we can do a data dump to the page tp make sure that the computed is working.
After getting our data to dump to the page we need to make a place for the data to render to from the map function.
we can use a v-for to iterate over the data and get it to render to the page correctly.
after getting the data to correctly render we can than go make a component holding our card that we want each pice of data to map over. 
after making the component we can then call on it in the page we want, but we have to use props, we can set up props in the component card.
to bring in an image we need to bind the :src=''.
when creating a computed to bind to, it has to have the exact value the style needs to be defined.
if its not bound properly nothing shows up.
inside of our model to reuse ot fro different data by using a v-slot
we need to make the ekement that we want to reuse as a component.
the slot is going to take whatever is inside of it and replace it with the content that was sent through the prop.
once we create the element we can add it to the slot.
the way we call it is <template #elementName> </template>.
when we use a router-link we need to put :to='{name:'' params: {}}'.
this allows us to navigate between pages without having to refresh the entire page.
we also need to make sure that we have a link to each route so that when we click on them they work.
when passing down data from a route we need use (route.params).
remeber that we cant mapp on a single object.
we need to use elvis operators when we have a null object in our appstate.
target=blank will open a link in a new window.
using target _self opens links within the same tab.
we can use $router.push({name:'',params:{}}) to push routes.
we use a v-model for forms it is a two way data-binding.
v-bind is one way binding.
https://prod.liveshare.vsengsaas.visualstudio.com/join?FC93D1AE23CFA97216B4E4AC096DE5729A28

# Fullstack Checkpoint Prep.

begin with express-vue project.
make project and cd into it.
open workspace first when opening vscode.
then quick intialize repository.
if we miss the workspace popup go to the workspace folder and open it through there.
next is setting up the enviorment, the env.js in both the server side and the client side.
then go to run and debug ans spin up both client and server.
go to localhost8080 to make sure that everything is running right.
then login to make sure the auth0 is working properly.
make sure we are getting 200s from the home screen making sure everything is connected.
next get post man set-up.
there are a set of tests already put in postman. and we need to make sure we make our back end to pass all tests.
The tests that are set up, need to be completed in there oreder that they are set up.
we going to a one-many and a many-many relationship in this checkpoint.
we should start with making a Schema modle in the server.Src 
make sure that we set up our schemas with the name:{type:,required: true, maxlength}.
for data that has multiple options we need to set up a enum, if use {lowerCase: true} with our enums we can make it so it is not case sensitive.
we can add a default img for imgs that migtht not get a cover Photo.
if we wanted a createdAt or updatedAt being brought in with our data on the front end we need to add timeStamps on the Schema.
then we need to set up populates fro any references that need to be connected through the schema.
we need to register evey schema in the dbContext
next ewe can start making a controller and a service. 
the fist function we need to make are the creates.
in the controller we need to have the our super set up with the api endPoint.
then the super we need to put our .use(Auth0) and our .post() function underneth it.
we need to have everything set up with async()req,res,next{try{}catch{}}
we need t omake sure if we are using the Auth0 we need to make sure we have our barer token is correctcly put in postman.
we can put our barer token in the top file in the variables slot.
we need to put the barer token in both value spots.
if set up propperly then postman should be able to act on the person who is signed in.
Make sure that we get the back end set up 100% befor moving in to the front-end this checkPoint.
Make sure that we are reading every error properly.
 virtauls and populates go hand in hand.
 reading the errors from postman is key fro passing this checkpoint.
 make sure that you refer to the UML diagram for the required data for the schemas.
 after making our creates we can then go on to making our .get() call above the .Use(Auth0) so we can get the data without being logged in.
 once we get our post working and our get working we can then run the whole file test to check ech test inside of the file, instead of individually testing each functin solo.
 the failed test titles are hints to what went wrong with the backend code.
 make sure if you confused about the populates you get help fast.
 when getting things by their ID we need to send to the service layer the (req.params.nameID).
 we need to make sure we have null checks in palce with an if(!name){throw BadRequest(bad)}.
 flipping a boolean: we need to send 2 things down to the service layer (req.params.albumId, reg.userInfo.id).
 Then in the service layer we bring in the (albumId, userId)
 we need to use another if statement.
 If we actually wanted to delete it we would do name.remove.
 but to flip the bool we doo name.archive = !name.archive await name.save() return name.
 we need the .save so the database knows that there was a change to the data.
params come from the url.make sure we do not move to front end until all tests in postman are done.
once the tests in postman are done make sure you get functionality on the front end done before getting crazy with the styling sauce.
make sure that we hitting the right endpoint in the crud methods being called in the super.
remember how we crossed our services in postIt backend to get the albums by pictureId.
we can even cross our function from our services to other services, services can call to other services.
but you cannot have a controller talk to another controller.
make sure that we are checking the naming conventins with the data coming back so we know it is coming back right.
make sure to reference to the filter bar in the PostIt app when working with the checkpoint.
we can use slots for our form intakes. 
like I did with the post if forms. 
then with that slot we can set up props.
if we make a componet with an opening tag and an end tag we can open it up and pass through our props into the componet.
we can use option tags with a vue form so there are multiple options to pick through on the form when creating.
if want the data coming in to come to flip the order of the array we can add a .sort() ay the end of
 the query and pass a parmeter in the sort for how we want the data to come in.
 the if we want the new created object to come to the top of the page we need to put an unshift on the formdata its self.
 in a virtual our local field is look at one of the fields on me.
 foriegn field is what oyu are referencing on another docment.  if you have 2 virtuals pointing at each other then you can get a count of both object with in the array.
 reference the member count in the postIt project to see how to cross populate.
 make sure that everything on the front end modle matchs everything on the backend.
 in the auth service there is a spot to add thing that might need to happen. like when you log in you can get any select data brought to the screen when the login has been verified.
 we can refrence other modles on the front end to each other. by using new ModleName(data.name)
 w can also in our prop alwo it to pass as what we are running though our modle and also have a OR statement with it being called an object to pass the data easier to other methods or functions trying to accses it.


