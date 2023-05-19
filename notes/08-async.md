simple async function with a resolve and a promise
vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv

Asyn cconst myPromise = new Promise((resolve, reject) => {
    let condition;

    if(condition is met) {
        resolve('Promise is resolved successfully.');
    } else {
        reject('Promise is rejected');
    }
});
const promiseToDoSomething = () => {
  return new Promise(resolve => {
    setTimeout(() => resolve('I did something'), 10000)
  })
}
----------------------------------------------------------------------------------
async await and return 
vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv

const watchOverSomeoneDoingSomething = async () => {
  const something = await promiseToDoSomething()
  return something + '\nand I watched'
}

const watchOverSomeoneWatchingSomeoneDoingSomething = async () => {
  const something = await watchOverSomeoneDoingSomething()
  return something + '\nand I watched as well'
}

watchOverSomeoneWatchingSomeoneDoingSomething().then(res => {
  console.log(res)
})
downloadPhoto('http://coolcats.com/cat.gif', handlePhoto)

function handlePhoto (error, photo) {
  if (error) console.error('Download error!', error)
  else console.log('Download finished', photo)
}
---------------------------------------------------------------------------
first example of form uplaoding using 1 function request or callback hell
vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv

console.log('Download started')
var form = document.querySelector('form')
form.onsubmit = function formSubmit (submitEvent) {
  var name = document.querySelector('input').value
  request({
    uri: "http://example.com/upload",
    body: name,
    method: "POST"
  }, function postResponse (err, response, body) {
    var statusMessage = document.querySelector('.status')
    if (err) return statusMessage.value = err
    statusMessage.value = body
  })
}
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
same thing but split between
VVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVVV
module.exports.submit = formSubmit

function formSubmit (submitEvent) {
  var name = document.querySelector('input').value
  request({
    uri: "http://example.com/upload",
    body: name,
    method: "POST"
  }, postResponse)
}

function postResponse (err, response, body) {
  var statusMessage = document.querySelector('.status')
  if (err) return statusMessage.value = err
  statusMessage.value = body
}



var formUploader = require('formuploader')
document.querySelector('form').onsubmit = formUploader.submit
-------------------------------------------------------------------------------------

this is a fetch and .catch function, when getting things from an api we want to make the promise of catch as a catchFail
for if theres an error in the system

vvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvvv
fetch('https://jsonplaceholder.typicode.com/todos')
    .then(function (response) {
        return response.json();
    })
    .then(function (data) {
        console.log(data);
    })
    .catch(function (err) {
        console.log("Something went wrong!", err);
    });

------------------------------------------------------------------------------------

we need to make sure both api are set up i our axios service
and update our api in the error handlers
one we are logged in we can and our socket settings are good we can dump the auth key and the footer for our project
first thing buid out our controller
export class namedController
then wire upp the controller into our ROUTER
then we dont need to worry about the router anymore for the rst of the app
newt in the controler we need to make a method to 
getNameFromApi(){
always followed by await and catch

}
 next we need to create out service and create another async getNameFromApi
 inside that we need our api/NameofArray
 once we can get our data logged to the console we can go to the app and make out empty array
the we can go back to our controller and create a appstate listener in the constructor to draw out array into the appstate
make sure to use capitalization when refering things to the router
we can use JOIN in our model 
data.desc?.JOIN('br/')
data,damage || 0 to day if there is no damage it sets the damage to 0
we can also use || '' to say if something isn't there leave it out
|| false when the data type is a boolean
the adapter pattern is what we don inside of the modal to represent how we want our data to be mapped
when we do a drawActive we don't need to do a template on it we can just setHTML directly
login button settings
get NameButton(){
  if(AppState.account)
  return 'login to add to spellBook'
}
return'<button>'
we use async when we add data to the sandbox
alwa
async get users spells(){
  try{
    await userSpell
  }
}
we use appstate.on (account, getspells) to listen to the login auth page
dont put things in the appstate till you need it, make sure to build your apps progessivly
use the data.prepared
type = "checkbox"
when we toggle we need to make sure that we call on the data id as the parameters in the toogle function
we have to use toogle on things that we add to the page that alreadu have a toggle feature happening
spell.prepared = !spell.prepared
this is flipping a bool^^^^^


--------------------------------------------------------------------------------------------------------------------

anytime we work with outh we need to go to our env.js file to set up our api retrieve system
alwys change your bse url in the axios service
first get a controller built and export const at the bottom
and always console log to make sure its hooked up
next we need to hook it up tp the router
you can just add our controller to the homeController with a coma
always read the docs before taking an api
use params{api_Key:} then plug in the actual key not the base url
we then get a our method working in the controller for drawing our data from the seected url and send it to the service
in the service we need to make hit tab on a method to send our export it
rember to test alot after seting up the getdata method in the controller and the service
there is a request limit on the dataUrls so be mindful of that
when we get a pojo instead of a whole array we dont need to actually map beacuase theres not a array to map over
setting null is a truthy falsy statement so seting somthing as null in our appstate 
document.body.style.backgroundImage = `url(${image})`
canst pic = appstate.namePic
css style class  ClassName: hover
date is an input type that will auto add a calender to the page
we can use the class of formcontrol in the  input div inide of a individual div itself
we use the ? as a queery selector
theres a big difference between onclick and onchange on change is used
let dateElem = daocument.getElementById
you can add a role=  button to make any test or icon a button
push to push data into a area
post to post data to an api
get to get the stored data from api


make sure we set up our env file
make sure you are using pop errors or pop confirmations


