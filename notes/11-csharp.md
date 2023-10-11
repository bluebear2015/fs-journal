# CSharp
c is a stricly typed lang.
variables in c#, you can  use var in c#. we also have to end every line with a semicolon ;
javascript has numbers, but c# has intergers.
best practice is to declare everything strictly with data type.
when we use these typs of data types we get very accurate intelasenses.
to instantuate a float the interger need to end in f.
when every there is a transaction using money we need to make it a decimal with a m at the end.
 a string has to be instanuated with double quotes,
 char have to be instanuated with single backticks.
 bool are true or false values.
 how we store collections in c# is array<int>[3] = new Array<int>[3]{1,2,3};
 lists work exactly like arrays in javascript. list<string> cats = enw List<string>();
 dictionaries work just like objects in js. dictionary<string, int> catDict = new Dictionary<string, int>(){{"cat",5}};
 list<string>.add("bob");
 list<string>.remove(0);
 list<T> is an ordered collection that allows duplicates and provides methods for searching, sorting, and enumerating its contents. 
 dictionarys are key value pairs and they look like this: Dictionary<string, int> myDictionary = new Dictionary<string, int>() { {"
 foreach (var cat in cats) {
    Console.WriteLine(cat);
    }
other c# syntax 
if statements: if (condition){do this} else{ do that}.
switch case statement: switch(variable){case "value": do something break; default : do nothing}.
for loops: for (int i=0;i<=5;i++){Console.WriteLIne(i)}.
while loop: while(true){}
foreach loop: foreach(){}
methods and functions: public void DoThis(){Console.WriteLine("hello world")}}.
classes: public class Cat{} inside which methods and properties go.
objects: objects are instances of classes.
interfaces: used to define a group of related methods. any class that uses this interface will have to implement these methods.
interfaces: they are like blueprints for classes.
namespaces: namespaces allow us to group code together so we don't have naming conflicts between different parts of our program.
abstract classes: abstract classes cannot be instantiated on their own. They must be inherited from by another class before being used. Abstract classes contain one ore
namespaces: namespaces help us organize our code better by grouping related things together into one place.
enums: enums are used when we want to limit what options an object can take on.
inheritance: inheritance allows us to create more complex classes from other simpler ones.
polymorphism: polymorphism means that an object may take on many forms and still behave correctly.
abstract classes: abstract classes cannot be instantiated directly because their purpose is only as a base class for other concrete classes.
abstraction: abstraction hides details so that only essential information needs to be known about them.
encapsulation: encapsulation refers to wrapping up data within one unit.
exception handling: try {} catch{} finally{}
anonymous methods: delegate() { //code here };
when using classes in c# you will rarley have code that is floating, almost all elements will go inside of classes,teh classes have constructors
calss{
(specify the type){
}}
all members are made with capitol letters, anythine it is going to be a method of function in a class.
the appSettings is going to be our envirmental files.
csproj is where all of our project dependencies.
appsettings.json file will contain sensitive info such as passwords etc..
the startup.cs is where our intial starting code is.
just like in javascript we will start with making a modle.
in the modle is where we need ot define what this object ;looks like in the dataBase.
we can add public ass an accsesor on a charetaristic in a object. making it public means that some can change it.
if we want to make it so people cant change the charectoristic of a object we need add a private callout on the object.
next we move to making the controller. we now  use a colon public class Controller: ControllerBase{

}
we can add a api call out with our route  above the class controller callout. [ApiController] [Route('api/Name')]
this is how you make your controllers.
now lets add some routes using get post put delete patch.
get route: [HttpGet]
post route:[HttpPost]
put route: [HttpPut("{id}")]
delete route: [HttpDelete("{id}")]
patch route: [HttpPatch("{id}")]
we also have access to HttpContext.Request.Body.ReadAsync();
route parameters: [RouteParameter("{id}")]
query string parameter: [FromQuery]
body content: [FromBody]
header values: [FromHeader]
form url encoded value: [FromFormUrlEncoded]
cookies: [CookieName]
session state: [SessionState]
request headers: [HttpContext.Request.Headers["name"]]
response headers: [HttpResponse.Headers.Add("name", "value");]
model binding: modelbinding happens automatically behind the scenes whenever we send something through HTTP request body or querystring.


how you define methods and functions in c# is different, we have to do alot more definition of the functions.
public string GetTest(){return"Hello World";}
we have to go the local host and accept the new route in order to hit the end point we made in the modle.
next we can make our service layer. we can call it public or private, but public is what we will be using.
while we can make our files inside the project but we can use nameSpaces to bring in variables from other files.
namespace projectName.modles
when we dont want our services to change inside the controller we need ot put private readonly.
we connect files together in c# using namespaces and global using statements.
namespaces are used to organize large projects into manageable parts.
global using statement allows us to import classes from other libraries without having to write out their namespace.
global using statement allows us to import classes from other libraries without having to write out their full namespace name every time they are called.
next we need to make a repository. at the top of the repositories we need to bring in our namespace using Name.model
namespace Name.repositories 
inside the repository file we need to add a public NAmeRepository(){
    _fakeDb = new List<cat>();
    _fakeDb.add(new Cat(1, "georgie", "orange", 5 false))

    _fakeDb.add(new Cat(1, mike", "black", 3 false))
}
then in our service we can connect the repository to the service.
when we are debugging we can look at the end of the "" brackets to see what it was held up on.
ActionResult is equivalent to a error response. the ActionResult will be what we are retuning after a method has been ran.
so if the method runs as intended it will return(whatWeWant) or it will return(bad request) using the ActionResult.
to run code first we just create an instance of the application db context and then seed data to it.
we need to make sure that we are adding the services.
services.AddScoped<catRepository>();
AddScoped<catService>(); 
we need to add this to the start-up file in this order to make sure the repository and the service are connected with the modle and the controller.
// This method gets called by the runtime. Use this method to configure the HTTP request pipeline.
inside the modle when we are setting the public or private of each data type we need to have public string Name{get; set;}
we use ()inside of our httpGet to append the url with a different end point. [httpGet("{catId}")]
then we can to the cat service.
c# does not use truthy falsey values. instead of (!name) we use (name == true) fro our truthy falsey logic.
a $ at the top of the string makes it so you can use {object} anywhere in the " in here  ".
if we wanted to get all cats from the database we would type out the following in our controller.
var cats = await _catService.GetCats();
ViewData["Message"] = cats;
this will return us back to our view page.
in order for us to access these variables outside of the scope of the current class we must declare them as properties within our model classes.
we can make methods wiht the same name but with different parameters to run the method for different actions that are used.
now lets start making some changes to our model.
first thing i did was remove my fake data because its no longer needed for testing purposes.
secondly I added a property to the class called Id which is set as key value pair.
thirdly I changed the name of the properties to match the names given in the json object.
we can use swagger to see the contents of an API.
look at the swagger page and learn how to use it and the tests properly.
making something as a singleton in the startup file will run and make the object that has been labeled as singleton only once.

Creating a table with c#.
create table hotdogs(
id INT AUTO_INCREMENT PRIMARY KEY, (the primary key is important for our auth?)
name VARCHAR (500),
imgUrl VARCHAR (),
bun VARCHAR (500),
dog VARCHAR (500),
description VARCHAR (1000));

INSERT INTO hotdogs
(name, imgUrl, bun, dog, hasKetchup, 
hasMuustard, description, price)
VALUES
('DogName', 'the New Img URL', 'The New Bun Type', 'the New Dog Type', 
The Ketchup Bool, The Mustard Bool, 'The New Dog Description', The New Dog Price)
If we want to get a something out of the dataBase we can use SELECT.
what comes after the SELECT is what column you are referring to.
SELECT * is select all
SELECT NameOfDataType to get a column 
we use FROM/WHERE to help specify what we want from our results.
SELECT name, price FROM TableName WHERE 'Bool' = true AND price < 6;
we can use LIKE 'NameOfDataType', we can use % as a wild card character to look for that word anywhere in the dataType '%NameOfTheDataType%'
There is alot you can do with the SELECT.
SELECT name, price, FROM TableName ORDER BY price DESC;
SELECT name, price FORM TableName LIMIT 2 OFFSET 1;
SELECT name, price FROM TableName WHERE price < 30 ORDER BY price;
 SELECT * FROM TableName WHERE id = SpecifiedDataTypeId;
 SELECT * FROM tableName WHERE Id = 
 DELETE FROM TableName WHERE id = SpecifiedDataTypeId;
 UPDATE TableName SET price = 20 WHERE id = specifiedDataTypeId;



 !IF WE MAKE MODS TO THE TABLE WE NEED TO DUMP THE DATABASE!
www.mysqltutorial.org
 WE DO ALL OF THIS IN THE dbSetup.sql




CREATE TABLE cars(
    id int AUTO_INCREMENT PRIMARY KEY,
    make ENUM ('tyoe1', 'tyoe2', 'tyoe3', 'tyoe4') NOT NULL,
    model VARCHAR(255) NOT NULL,
imgUrl VARCHAR(500) DEFAULT 'default pic img',
description VARCHAR(100),
isNew BOOLEAN DEFAULT false)
^^^^THE TABLE MODEL FOR A CAR^^^^^^^^^

vvvvvvTHE WAY TO MAKE A CAR USING THE TABLEvvvvvvvvv
INSERT INTO cars 
(make, model, year, price, isNew)
VALUES
('type1', 'modelName', 'newImgUrl', 'NewDescription', false);


inside the of the AppSettings.Development.Json we need to connect ourselves to the database.
in the connection string we need to put our ScaleGrid info.

after we have made our table and created some Data using the table data types, we can make our model.
in the model we need to set the nameSpace, 'namespace server.model'.
the we set the class as public then make our data stucture model. 
public class className{
dataTypes for the model.
}
next we can make a controller with the [httpREQ] with the request we are wanting to make to the api.
from the car controller we need to make sure that the repositroy is registered for our [httpREQ]'s.
then we can maek our service. we need to make sure that the controller is linked to the service that is linked to the repo that is linked to the model.
next we need to go to our startup page and register our service and our repository.
in the service we need to bring in our nameSpace, and inside of the class we need to bring in the private read only Repo stuffs.

inside of the repository to connect it to our mySeq.
internal LIST<ModelName> GETfunction(){
    string sql = "SELECT * FROM tableName"
    List<modelName> cars = _db.Query<modelName>(sql).ToList();
    return cars
}

[HttpGet($"nameId")]

public ActionResult<modelName> getById(nameId)



then in our service
internal car getById(int carId){

}


then in our repository
internal car getById( int nameId){
    string sql = $"SELECT * FROM tabel Name WHERE id = "@nameId;";
    modleName name - _db.Query.(sql, new {nameId}).FirstOrDefault();
} ^^^ this is a way of itterating through an array but comparing the data to the keyId that we have passed to it"@nameId"
we do this so to avaoid, SQL injection atatcks, pass a {key:value} into the Query to matcha nd pull the object that matches our {key:value}.

next we cann go back to the controller to make our [HttpREQ] then from there we can take it the service layer for more defining on what we want to do with this REQ.
then we can go to hte repository to finish out the the REQ.

we can call other methods inside of the service layer to get dataTypes that have already been declared like: removeName(){
    getById(nameId) to get the car Id from the method that already has it
}


in our repository, we can see how many rows we affected by using 
int rowsAffected = _db.Execute(sql);
if (rowsAffected > 1) throw new Exception('this is not good');
if (rowsAffected < 1) throw new Exception('nothing happened');


next we will learn how to do i put request to edit something.
[HttpPut("NameId")]

public ActionReslut<modelName> UpdateName(int nameId, [FromBody]modelName updateData);
try{
    UpdateData.Id = NameId

}catch{
    error
}

then in our service we can
internal modelName Update(modleName updateData){
    car original = this.getCarById(updatedData.Id)
    original.dataType = UpdateData.dataType !=null
    _repo.Update(original)


}

we can make dataTypes nullable by going into the modle and adding an Elvis opperator to the data type that needs this data type. so if its interger it will need an elvis operator.


----Making Many to Many relationships, using auth0 With C_SHARP---------
First wew start the project using dotnet-vue. 
then we need to enter our workspace in VsCode.
Then inside the project we need too set up our enviormentals.
In the appsettings.development.json inn the connection string is were we need to put our database 
info.
to be able to get info from one table to another table we need to use sequelQuery.
next we need to go to our client and set up our env.js file then we can spin up the client.
(now that we are using c# we need to be aware of our base URL to the correct port).
we then need to go back to our appsettings.develope.json and add the Auth0 domain, and Aunt0 client.
next in the dbSetup.sql, we can create table.
to have TableData reference other TableData, we need to tell the Table that the dataType is pointing to Differnet Table.
creatorId VARCHAR (255) NOT NULL
FOREIGN KEY (creatorId) REFERENCES accounts(id) ON DELETE CASCADE
The FOREIGN KEY is what is letting us point to a column on a seperate Table.
we can also set up triggers that will wathc if something happens and it is tied to the data we have 
(ON DELETE CASCADE)
SELECT * FROM TableName JOIN accounts;

Break up the data you want to make sure you know what tables you want to get info from and what i want from that table.
SELECT alb.*, act.name
FROM TableName tbl
JOIN accounts act ON act.id = alb.creatorId; 
WHERE TableName.id='idNumber'; or
WHERE TableName.DataType = 'DataTypeName';



first after getting the tables set up in our dbSetup.sql, we can then make a model.
In the model we need to set the namespace for the model.
We then can make a repository. in the repository nedds a namespace adn then we need to make the repository public.
then from there we can make our service. the service needs a namespace and we need to make the service public and connect it to the repository.
Next we can make our controller. 
Next we need to register our services in the Startup.cs.
 after getting all the model, repo, service, controller set up we can start our CRUD requests inside of the controller.
 in the modle we can add on whole model in the model of another object.
 then inside the repository we can specify on what we want back with the get.
 inside the _db.Query<tableName, Account, tableName>(sql, (album,ccount)=> 
 {
album.creator = account;
return album;
 }).ToList();

 to bring in Auth0 into c# we need to bring it in as a private read onlyin the header.
 inside of the method we want ot use the auth0, 
 Account userInfo = await _auth0.GetUserInfoAsync<Account>(HttpContext); 
 albumData.CreatorId = userInfo.Id;
 
 we also need to wrap the public action result in a Tack<>
 anytime we use asynchronis methods in c# we must use Task<>
to use the auth0 on a [HttpREQ] we need to put it above the REQ callout.
we can even add it to the top of our controller to have any instance of REQ run through auth0 first.
[Authorize]
[HttpPost]
flipping a bool. or a soft delete.
we use a delete request even though it is an edit to the info.
[Authorize]
[HttpDelete("{albumId}")]
public ActionResult<TableName> FlipBool(int dataTypeId){

}

