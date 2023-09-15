# Async

some API's, need a key to get access to the data they store.
make sure to register the controller in the router. then move on to making a modle.
and then we can make our first get request and do a data dump to the page.
inside of our get requests there always need ot be a try catch.
after the router we need to make sure our axios service is set up the right way.
inside our service above our class we put the const = axios.create(){}.
this will allow us to use this instance for all of out api calls.
then inside that create method we have to add an interceptor.
the interceptors are used when you want to run some code before or after your call has been made.
every thing that is async gets a try catch as well.
every time we make a post request we need to put the url endpoint.
we also need to send it with the body of what we want to send along with it.
if something goes wrong while sending the information back from the server we can throw errors here too.
first make sure your connection string is established between postman, mongo, and vsCode.
but properlly setting up your mongoDB.
next we can build our models, using Schemas.
schemas help define how our database looks like so we know exactly whats going into each collection/table.
in order to connect them together we need to import mongoose.
mongoose allows us to interact with mongodb through node.js.
once connected we can start building schemas.
each schema needs at least one field which represents its primary key(id).
after making a schema we need to go register the schema in our DBContext.js file.
in order to refernence a schema in another schema we need to call the the schema in the type section.
now we can finally start creating our controllers!
controllers take care of getting info from the dbcontext layer downwards.
they handle any logic needed to process the data coming off the wire.
we need to add virtuals to schemas that are calling another model inside of it.
so if i had two different collections called users & posts.
i wouldnt want my user schema to contain every single post in their posts array.
instead I could just tell Mongoose to only return the id property of those documents instead of returning everything.
instead I could just say "userSchema.virtual('posts', {ref: 'Post'})"
to tell Mongoose that whenever someone wants to see the posts of a certain user he should look in Post Schema.
this means whenever someone tries to pull the posts property off of a User object it will return only those Posts objects that belong to said user.
which means whenever someone asks me for a list of users, give me only those who have 1+ posts associated withthem.
that means whenever someone tries to pull the posts property off of a User object it will return only the Posts objects that match thier id.
that way only the id of the post is stored in the user document but not the whole object itself.
to actually save the new changes to the db we need to use .save().
idealy a turnerary is used when flipping a bool.
for example instead of saying 1 === true || false;
you should write 0 !== true && !false;.
404 error stands for Not found.
500 error means internal Server Error.
402 error means Unauthorized.
200 means success.


# Hackathon prep

we are using mvc express. this contains a server and a client.
when we start working in mvc express we need to make sure we open the workspace if we are not inside the workspace it makes it so we do not have access to the project at the correct level.
then we need to set up our server env and then we need to set up our client env files.
make sure after setting up the env files we need to spin up the client and the server.
when working on the front end we dont need to worry about reloading the page because webpack takes care of everything behind the scenes.
when doing npm install on both sides there might be issues because they may be trying to download packages differently based on where you're running them.
to uses middle wear you put .Use((req, res, next)=>) next().
we use .use(Auth0Provider.getAuthorizedUserInfo)
this will allow us to access the auth0 token on the req objecct.


---------connecting the front end----------
first thing we need to do make sure that the auth0 is working properlly from the back end code we made.
the first step was to create an account on Auth0.com website.
remeber on the front end we need to register all our controllers in the router-view.


coderDatingSite.
