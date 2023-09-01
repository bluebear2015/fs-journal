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

