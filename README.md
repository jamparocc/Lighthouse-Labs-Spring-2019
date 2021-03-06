# Lighthouse-Labs-Spring-2019

21-Day Coding Challenge Welcome to the Lighthouse Labs 21-Day Coding Challenge! Over the next 21 days you’ll be travelling aboard the exploratory vessel ISS Lighthouse, on a mission to explore the galaxy.  Just as you depart the solar system, a gigantic space bug knocks you off course! As the ISS Lighthouse captain, you’ll need to solve daily coding challenges to repair the ship and continue on your mission.  Remember: We only release ONE challenge a day but you can now catchup to the current challenge if you fall behind.  Click on the flashing radar below to start the first challenge. A new challenge will be unlocked every day at midnight PST. Complete all the challenges until the grid below is completely filled. Have fun!

## Challenges 

https://coding-challenge.lighthouselabs.ca/

### Global objects

There are a few objects you're going to be working with and their initial values. This is only a subset of them, to give you a idea of what they look like. You can see below that they're all messed up:
```
var navigation = {
  x: -2,
  y: "Banana",
  z: "Beep",
  speed: "raaaaid"
};

var ship = {
  powerOn: false,
  modules: [],
  antenna: {
    active: false
  }
};

var radio = {
  frequency: "Kenneth",
  message: "Bugs are cool.",
  beacon: false
};
```

## Challenge #1
You are the captain of the exploratory vessel, the ISS Lighthouse, on a mission to explore the galaxy. Just as you depart the solar system, you encounter a gigantic space bug, which knocks you off course! Now you're lost in space, your radio and navigation are out, and it's up to you to work with your computer to get things going again.

Fortunately, your ship enabled your LARRY (Language-Aware Repair Robot of the Year), when the systems went offline. For some reason, the engineers who created LARRY made him duck-shaped, but he is very good at doing exactly what he is told to do. He has a terminal on his back that lets you use JavaScript to make changes to the ship.

Your job as captain of the ISS Lighthouse is to use your JavaScript skills to talk to LARRY and get your ship back in working order! You've got 21 days to fix the navigation and radio before the command centre back on Earth gets worried and launches another ship to come looking for you.

"POWER OFF!" quacks LARRY. That sounds like a big problem! You should probably get the power back on, otherwise things are not going to go very well for you in the depths of uncharted space! Unfortunately, the manual for your ship is hard to read in the dark.

"Ship's powerOn property set to false!" LARRY exclaims. "MUST CHANGE VALUE! QUACK!" Okay, that sounds pretty serious. Fortunately, you remember from orientation that there are things called "properties" in JavaScript. You access properties using the '.' operator. With just the light from LARRY's terminal, you need to write a function called ```powerOn()``` which will change the 'powerOn' property of the 'ship' object. If that's set to 'false', changing it to 'true' should get things going.

**Hint:** LARRY loudly quacks out, "Set values in JavaScript using a single equals sign."

>**Hint**
>
>This challenge is about creating a Function and working with an Object Property in JavaScript.
>
>**On Functions:**
>
>[How to define functions in JavaScript](https://www.digitalocean.com/community/tutorials/how-to-define-functions-in-javascript)
>
>[CodeCademy tutorial on Functions](https://www.codecademy.com/courses/learn-javascript/lessons/functions/exercises/intro-to-functions)
>
>**On Object Properties**
>
>[Digital Ocean](https://www.digitalocean.com/community/tutorials/understanding-objects-in-javascript#adding-and-modifying-object-properties)'s tutorial on modifying object properties.
>
>**Example of Global objects available**
>
>Look for the "Show Global Objects" link right before the challenge number on this page.
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)


## Challenge #2
The lights flicker on, and you can see the interior of the ship, along with LARRY, your duck-shaped friend. You feel relieved, until LARRY’s eyes start to glow red, and he starts blaring, "SHIP IN DANGER! SHIP IN DANGER!"

What can it be? You've turned the power back on, everything should be back to normal, right? "MODULES NOT ACTIVE!" Modules, what modules? A quick check of the ship's status board reveals an empty array labelled 'modules'.

You flip through the manual to the section labelled 'Modules', where the first page describes a number of available modules. They are stored in memory in the ```availableModules``` array. Each module is an object, with four properties:

the ```name``` of the module is a string
the ```size``` of the module is an integer
the ```enabled``` and ```essential``` properties are booleans
Start off by finding out how many modules there are. Make a function called ```countModules``` to reveal how many modules there are to choose from.

>**Hint**
>
>While there's a lot of information about the module here, the simple challenge is to find out how many modules there are. They're stored in an array, and what we need is to find out how long the array is. Check out these resources:
>
>Here are some Digital Ocean tutorials on [Understanding Arrays in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-arrays-in-javascript)
>
>You can also work with arrays on [CodeCademy](https://www.codecademy.com/courses/learn-javascript/lessons/arrays/exercises/arrays)
>
>Khan Academy also has some good exercises that you can do [here](https://www.khanacademy.org/computing/computer-programming/programming/arrays/pt/intro-to-arrays)
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #3

"QUACK QUACK QUACK QUACK QUACK QUACK QUACK", goes LARRY, his eyes still glowing red. He’s counting off each of the seven modules on the list - you must be on the right track! Now to find out how many of them are essential.

Use your JavaScript skills to write a function called ```countEssential()``` which will count how many modules from the ```availableModules``` array have the essential flag set.

>**Hint**
>
>This is a bit more complex. We need to loop through the array, and count how many of the modules have the essential flag set. You'll probably want to make a new variable to count the number of essential modules, and then you're going to build a loop. Here's some resources on looping:
>
>- [Learn about Looping](https://www.digitalocean.com/community/tutorials/how-to-construct-for-loops-in-javascript)
>
>- You can also check out [CodeCademy](https://www.codecademy.com/courses/learn-javascript/lessons/loops/exercises/loops)
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #4
"DANGER QUACK DANGER QUACK!"

LARRY seemed so happy before, but he really is starting to get a bit agitated. Now that you know there are three essential modules, maybe you should start loading them into the ship's systems.

Write a function called ```loadModule()```. It needs to take a parameter, called ```index```. Your function should be set up like this:

```function loadModule(index) { }```

When ```loadModule``` gets the index number of a module, it should load it into the ship's ```modules``` property (which is already an array). Before you load it in, set the ```enabled``` property to ```true```. You need to loop over the availableModules and find the module called "life-support" and get its index, then use it to call ```loadModule()```.

**Hint:** You need to either loop through ```availableModules``` outside of any function or write a seperate function that handles the looping make sure it is called in your code"

>**Hint**
>
>Oh my gosh, there's a few steps here. First, you need to make a new function. We've done that a few times now. Then you need to get that function to do three things:
>
>**1.** Find the module by its index
>
>**2.** Set its ```enabled``` property to ```true``` (Remember setting object properties from challenge #1?)
>
>**3.** Add that module to the ship's ```modules``` array.
>
>The first step is easy, because you just need to access the ```availableModules``` array with the index, using the [] notation. For the second step, use the same strategy you used to turn the power on in Challenge #1. The last step uses a method called ```.push()```. You can read up on how array pushing works [here.](https://www.digitalocean.com/community/tutorials/how-to-use-array-methods-in-javascript-mutator-methods#push())
>
>Also, don't forget to find the index of the ```life-support``` module and use your new ```loadModule()``` method to activate it!
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #5
"BREATHE EASIER!" LARRY quacks out. "LITERALLY. Life support module loaded. Propulsion needed."

You can re-use your code from before, but this time you should do what all good programmers do: modularize your code. Write a function called ```findModuleIndex()``` which will take in a name that you’re looking for, and return the index of that module in the ```availableModules``` array. Remember: it has to have the ```essential``` flag, too!

Use your ```findModuleIndex``` function to find the "propulsion" module and then load it into the ship's system.

>**Hint**
>
>The good news here is that if you succeeded at the last challenge, you've got all the logic you need to do this one. Remember the work you did to find the ```life-support``` module's index? Write a function that does that when you pass it the name of the module as a parameter.
>
>**Hint:** Make sure you are building on top of the last challenge. ;P
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)


## Challenge #6
"NAVIGATION SYSTEM needed," LARRY tells you. Navigation is important - you can't move through space without it!

Use your already-defined methods and load in the "navigation" module. It's pretty simple once you have the functions to do it, and LARRY's eyes are finally easing from red back to normal.

>**Hint**
>
>Great news, you have the ability to find a module's index. We need the navigation module's index, and then we want to load that module in, by index.
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca)

**Challenge 7 Global Objects**

```var navigation = {
      x: -2,
      y: 4,
      z: 7,
      speed: "raaaaid"
    };

    var ship = {
      powerOn: false,
      modules: [],
      antenna: {
        active: false
      }
    };

    var radio = {
      range: {
        low: 88,
        high: 108,
      },
      frequency: 0,
      message: "Bugs are cool.",
      beacon: false
    };
```
   

## Challenge #7
You look over at LARRY, expecting him to quack out his next prompt, but it seems LARRY is now the one malfunctioning! You open up the manual, and find the section on LARRY. Apparently, loading modules can sometimes cause LARRY to get stuck in an infinite loop.

You can fix him, you'll just need to write some code! Write and call a function called ```resetLARRY()``` which will prompt LARRY to quack ten times so he breaks out of his loop.

There is a function called ```LARRY.quack()``` that you can use in your code.

>**Hint**
>
>Okay, the hint here is that we have given you the method you need to make Larry quack. You just need to make a loop. This loop needs to run ten times, calling the LARRY.quack() method we've given you. Here is the material on loops again on Digital Ocean.
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #8
The little duck-shaped robot shudders back and forth for a moment, and his eyes flash as he releases a barrage of ten quacks. "Thank you!" he exclaims.

"COMMUNICATION MODULE NEEDED," LARRY blares suddenly. He repeats it twice more - he’s rather insistent! Luckily, you've got the code for this. Load the module called "communication" using ```findModuleIndex()``` and ```loadModule()``` from before.

>**Hint**
>
>Now we are back in business! Let's go back to using ```findModuleIndex()``` and ```loadModule()``` to get some communication going!
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #9
"QUAAAACK radio beacon not sending!" Now that LARRY is reset, he can't help but point out all the things wrong with the ship. The radio beacon is important - it’s the part of the ship that relays messages to Earth about your location and welfare. Resetting it is a two-stage process: first you need to set the message. The message needs to contain the current state of the ```navigation``` object.

This is where you learn about something called JSON. JSON stands for JavaScript Object Notation, and it allows us to express an entire JS object as a string. There’s a built-in function in JavaScript that will take in an object and turn it into JSON. That function is ```JSON.stringify()``` - if you pass your object to that function as a parameter, it turns into a string.

You need to write a function called ```setMessage()```. This function should set the ```message``` property on the ```radio``` object to be the JSON version of the ```navigation``` object. Don't forget you need to call your ```setMessage()``` function.

>**Hint**
>
>Looks like we've got to make a couple of steps now to get going. You can [read the docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify) here on how to turn a JavaScript object into a string using ```JSON.stringify```. There are some good examples there for you.
>
>Think about the order of things you need to do:
>
>- Make a new function called ```setMessage()```
>- Within that function, you need to access the ```message``` property of the ```radio``` object (Remember you can do this using the '.' operator)
>- Then you need to make sure you are setting ```message``` property to the JSON version of the ```navigation``` object
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)

## Challenge #10

"Beacon not sending!" LARRY is still blaring, and it’s time for step two: activate the beacon.

You check out the radio object, and see that it has a 'beacon' property. Now that the message is set, write a function called ```activateBeacon()``` which will set the ```beacon``` property to ```true```.
>**Hint**
>
>This should be a cake walk now for you. Write a new method, and use that method to change an object property.
>
>[Click here to access the Help Forum.](https://21day-forum.lighthouselabs.ca/)
