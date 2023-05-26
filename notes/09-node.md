# Node

-------------------------------------------MONDAY APRIL 23------------------------------------------------------------------

server side concerns
the serverside also follows the mvc pattern
the database connects to the server with the user
but the database should not interact with the user before interacting and passing through info to the server

befor creating our own template we need to npm i -g bcw
the use the node-server-author
express library -- -- --
the client file is used to build your clients
in the package.json inside is what looks like a java sxript object but inside our our dependencies 
inside is the extra librarys we use to make life easier on the backend
express is the core library we are using while runniing our backend server using node
mongoose is the library we use to talk to our database
sockets.io is used for live chats
dev depencies are there to make sure your writing your code directly
to access your dependencies you have to be in the same directory that you have the package.json and then run the npm i in the terminal
it will then install all the librarys needed for the one project be written
to execute some
inside the 
index is basically the adapter that allows us to use the import export
we still need to setup our .env file with our auth codes but dont need to use quotes inside the env file with node
port 300 is a fake server ser up for deveoplment
port 8080 is the user interface
the whole purpose of theus is to reach an endpoint that we can
in the ca;ie controller the case controller is how we set up connections and stuff
inside the super(the enpoint) it is the base endpoint for our controller its our mount path which is  th correct term
insted of using on we use gert
remeber that the .get(if this event happens do this function)
('',function) means if there
after making anychanges in the server you need to respin it by hotting the play button in the right hand side
req. = request
wehn you start a file you need to export class extends basecontroller
make a constructor with a super inside of it and inside the super is going to be our endpoint
then this.router .get('',this.method name)
next make out the method the params of that methoud needs (req, res, next)
with our try catch we need to put next(error)
we can see the console on our begug console screen
insted of colsole.log in node we use logger.log
.get('') this is calling on our supers params as our own
.get('/:placeholder',this.)
res.;body is what all formdata takes place
when ever a request a post or put you will be dealing with the body
bcw create express-mvc
once we get our project into vs code we can go to our node file and click upen window
after selecting the file and then we need to open the file outside of the workspace
then we need to put our env info in which is what we saves in my notes
including the connection string
next we move to the client folder and we need to do the same thing inside of the client domain in the env file
these are responsible for linking these two things together this makes it so our client and server are pointing at the same end point
we want to make sure we are in our client file befor we bcw serve
the network tab is gong to be our best friend when making requests to our database
inside the mongodb is where we are going to store our data in the database
we need translators between differnet framework languages
we go this by passing through our code by using mongodb
schema and model are the samething
we need to import mongoose inside our schema and our model
typically you always want to put required in all out properties
anytime we have textbox options we need to make saftey nets so that malicious users cant take advantage of things
we then register out schemas tp the database in the dbContext file
next thinf we need to do is make our cars and our service
we need to put extends Basecontroller on our controllers form now on
dont forget to put a super inside of the constuctor in the controller file
inside postman we need to create new collection
in postman we can creat a varieable for our base URL so we dont have to write it 
middleware is the middle man between the user and the controller
we put our authGuard in the super and anything below that is going to have to be authorized befor that function get called so where the functions lay inside that super are really important
in the authorization selection in postman we can go to the varibles and create an new veriable  and create a bearer token variable then we go to the authorization and mark it as bearer token
but we are going to need the nearer token to use the api after declaing ony verified users 
make sure to make a request in postman you need to go to body then raw and set the language to JSON
using the timestamp true in the schema will make it so it has an updated created at time
a testing suit is collection of folders that make it easier to test functionality of the written code
whenever we do an edit we need to do a null test we need to verify if the car being editted is the right id
null checking is throwing an error if there is no car in the database that matches the ID
if we ever need a referebce for editing reference gregslist
null coelesence is making sure the 
when we handle null coelesence with a boolean we need to make a fubection that can flip the boolean
example. originalData.param = newData.param ? newData.param : originalData.params
null coelesense make it so if you edit one piece of the givin array it we default to the original data that has not been edited
a git request should always be able to facilitate a query selector a query comes in as a request
query and parameters are key value pairs
if you try to pass an argument you need to format it as an objest
make sure to just add querys to all get requests


--------------------------WEDNESDAY------------------------------------
lucidChart   lucid.app
what does enum mean enum means many so under the hood its its a string but really it has a preset variable that it can be
a many to many need a middle function to bring the two data types together
virtuals allow us to grab correlating arrays that we want to pull data from
restful api connections
when doing a many to many we need to make callout to the data we want to see in the model
when we go to our client we can bcw serve and create our bearer token
then we need to go to our network tab and open the account and thats where we will get our bearer token
then in postman we can go to authorization and paste our bearer token info
after getting auth0 set up in our constructor we can then put a validate method inside of the desired function that need to validate Ids
for creats populate gos on a new line. ORDER MATTERS.
keep in mind were the relationship between the data you want is coming from to make the functions and methods in the appropriate path


