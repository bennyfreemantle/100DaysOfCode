# 100 Days Of Code - Log

### Start date: 26/09/2022

### Day 1:

**Today's Progress**: psuedo-classes are tricky!

**Thoughts:** Today was my first day starting The School of Code cohort 13. As well as my 1/100 days of code. Playing around and completing all [CSS Diner](https://flukeout.github.io/) tasks. Pseudo-classes are tricky! I found working backwards helped understand them a little better. Nevertheless will likely still require mdn lookups for future usage.

---

### Day 2:

**Today's Progress**: Git commands & Hack The Galaxy

**Thoughts:** learned a few more Git commands and was humbled very quickly with the Hack The Galaxy problems. Critical and computational thinking is a skill I will undoubtable need to work on. Luckily, throughout my journey with SoC I will be exposed to plenty more problems to try and solve which i will carry through into my career.

---

### Day 3:

**Today's Progress**: JavaScript basics

**Thoughts:** Had a refresh on the JavaScript basics. Primitive types, functions and loops. Created a very basic password checking system with 3 tries and you’re out. Finally, helping others, helps me ALOT.

---

### Day 4:

**Today's Progress**: JavaScript basics continued

**Thoughts:** How to approach receiving / giving feedback & the importance it has.
Refresher on JS Objects and Arrays & how to add, remove, read and update them.
Polishing up on the pair programming git clone, add, commit, push, pull work flow.

## Key Concepts

- Objects can be accessed with either . or [ ] notation
- Can only reference object key’s that are Numbers with [ ] notation as . would cause a syntax error
- As mentioned above with Array's the indexes are always numbers so we use [ ] notation when trying to access array values.

```js
let myArray = ["Hello", "World"];
myArray.1; // Syntax error
myArray[1]; // World
```

- Arrays start at index 0
- You would loop over an Array with a for loop 99% of the time instead of a while loop.
- typeof []= “object”
- Because Arrays are Objects they have ‘pre-baked’ methods and properties you can use out of the box.

```js
// Declare an array
let array = [];

// Add to an array
array[0] = "hello"; // update at index 0
array.push("world"); // add onto the end of the array
array.unshift("before"); // add at the start of the array

// Remove from an array
array.pop(); // remove from the end of an array
array.shift(); // remove from the start of an array

// remove from a defined starting index in the array
// 0 = the index to start removing items from
// 1 = how many items to remove
array.splice(0, 1);

// Declare an object
const object = {
  age: 25,
};

// Add a key:value pair into an object
// Can also be used to update an exisiting value
object.myName = "ben";
// Remove from a key:value pair from an object
delete object.age;
```

---
### Day 5:

**Today's Progress**: Hackathon Friday

**Thoughts:** Our first Hackathon working as a pair. Pushing and pulling our changes to each other, taking it in turns to write up each task.

## Key Concepts

- Push, pulling git workflow is picking up speed
- Plan, plan, plan.
- Google is your friend, always ask it for help.

---

### Day 6:

**Today's Progress**: Finishing [Hackathon Project](https://github.com/bennyfreemantle/w1_hackathon_rock-paper-scissors-git-test) & Refactoring

**Thoughts:** Refactoring code is frustrating. Finished Rock paper scissors app on my own forked repo. At times I wasn't sure why it wasn't working, breaking it down and trying another way helped alot. I kept making silly mistakes by leaving old variables and function calls which caused my app to behave in unexpected ways. Even if the code was logically correct.

## Key Concepts

- Functions doing only 1 thing
- losing my mind after an hour of debugging it was because I had called the function twice…


#### Extension 2: The Clairvoyant Computer plan / pseudo-code
```js
// Extentsion 2: The Clairvoyant Computer
/**
 * How would you go about making the computer win every time ?
 * 
 * You could change the way the computer chooses it's option
 * instead of choosing based on a random number, it would know what you had chosen before
 * by reading your value first.
 * It would then choose the 'opposite' option to beat you everytime
 * 
 * you could store these 'opposite' pairings in an object
 * 
 * let clairvoyant = {
 *  rock: 'paper',
 *  paper: 'scissors',
 *  scissors: 'rock'
 * }
 * 
 * The computer would then access clairvoyant.userChoice as the computers choice
 * so it would always choose the 'opposite' that beats the player 100% of the time
 * 
 * 
 * 
 * 
 * How would you go about making it so that the computer wins more often
 * 1/2 the time, 1/4 of the time, 90% of the time ?
 * 
 * using the implementation above, you could now add a random number generator
 * to decide if its going to 'cheat' or not cheat. It's always the computer that gets
 * to decide if they win or lose. And not luck.
 * 
 * random number 0 - 1 : cheat - don't cheat = 1/2 chance
 * random number 0 - 3 : cheat - don't cheat = 1/4 chance
 *  random number 0 - 9 : cheat - don't cheat
 *  for 90% you would need to inverse the odd's so if the roll was between 0 - 8
 *  the computer would win, 9 rolls = 90%
 *  if the roll was 9 and only 9 the computer would let the player win giving the player
 *  10% win chance.
 * 
 */
```

---

### Day 7:

**Today's Progress**: Rest & Research

**Thoughts:** Slow day today, mostly recapping what I did last week and researching string and array methods and how to use them.

## Key Concepts

- forEach array loop
- slice() string method extracting specific parts
- replace() as the name suggests, replaces some or all that match a pattern

---

### Day 8:

**Today's Progress**: The JavaScript DOM

**Thoughts:** The DOM is a JavaScript object representation of HTML, and not the HTML itself. It can be manipulated in many ways. Reading, writing, adding & deleting elements. Can start to fully see the power JavaScript has outside of just the console.

## Key Concepts

- How to read, write, delete and add elements from the DOM
- querySelectorAll() method returns an ‘array like’ object called a NodeList
- You can iterate over the NodeList and execute code on each item. Just like you can with an array.
- console.dir() function is useful to visualise and see the object and all it’s properties
    - displays an interactive list of the properties of the specified JavaScript object.

```js
// Point to the html #user-name and store the result into userName variable
let userName = document.querySelector('#user-name');

// Update the textContent of userName to = 'ben'
userName.textContent = 'Ben';

// Create a new element
let newDiv = document.createElement('div');

// Change / add content to the the new div
newDiv.textContent = "I'm a fresh new div element";

// Append the div to the body (will append as the last child)
document.body.appendChild(newDiv);

// Remove the div from the DOM
document.body.removeChild(newDiv);

```

---

### Day 9:

**Today's Progress**: The JavaScript DOM Continued & addEventListener()

**Thoughts:** Continuing from yesterday, working with the DOM and implementing addEventListeners to a starter RPS project. We also had a previous bootcamper come in the morning and give a quick talk to help reassure, that what we might be feeling is normal and being flooded with information isn't necessarily a bad thing. We just have to keep working and building things with our prior knowledge, and laying need bricks on top of it.

## Key Concepts

- An event is an object
- on every DOM node object ‘addEventListener’ method exists
- addEventListener(arg1, arg2) takes in 2 arguments
- arg1 == type of event js needs to listen for ‘click’, ‘mouseover’
- arg2 == the function called that contains the code we want to execute
    - callback function, the definition of that function
- event.target.value to read value

```js
// gets the id #user-name from our DOM
let userNameInput = document.querySelector('#user-name');
// adds an event listener to our #user-name id
// listens when the user 'keyup' on our element
userNameInput.addEventListener('keyup', updateOurUsername);

```

---

### Day 10:

**Today's Progress**: Fetch(), Async & Await & the Call stack

**Thoughts:** Today was all about asynchronous JS and awaiting for it to resolve.
I also learnt some useful functions provided to us by the browser API.. setTimeout(), setInterval() and how to combine these with the JS Date object to create a real time working clock.

## Key Concepts

- [Call Stack](#call-stack)
- JS is synchronous by default meaning it reads from top to bottom
- setTimeout(arg1, arg2)
    - takes 2 arguments
        - a function to ‘callback’
        - time delay in milliseconds
- setInterval
    - allows us to run a block of code over and over at a set time interval
    - similar to setTimeout() it takes 2 ‘primary’ arguments. A callback function & a time delay in milliseconds
    - we can use clearInterval() to stop our setIntveral 'loop' from running.
    
```js
let count = 0;
// using an anon function, could also use => syntax
let countUp = setInterval(function() {
  // increase our counter by 1 every second
  count++;
  
  if (count === 5) {
    // Stops our countUp interval timer if count === 5
    clearInterval(countUp);
  }
  // log out our count
  console.log(`our count is: ${count}`)
  // 1000 milliseconds = 1 second
}, 1000)

```

### Call Stack

- orders of instructions we give to execute in order
- setTimeout creates a separate queue - Callback queue
- once the elapsed times passes, an event loop executes
    - prioritises the function in the call stack and slots it back in to the top

![call stack and event loop](https://miro.medium.com/max/1400/1*iHhUyO4DliDwa6x_cO5E3A.gif)

### Fetch()

- visits an external link and ‘fetches’ its content
- fetch returns a promise so we need to await it
- comes back most commonly as a json object
- we need to await our data.json() to parse into a regular object
- access our object using . or [ ] notation

```js
// async function expects an await
async function foo() {
	// fetch some api end point returning json
	let response = await fetch("https://api.kanye.rest");
	// useful to check its done good
	if (response.status == 200) {
		// our response was successful
		// do our code
		// get the json out of the response and await it
		let data = await response.json();
		// log our data
		console.log(data);
		let quote = data.quote;
		// log our quote
		console.log(quote);
	}
}

foo();

```

---

Continuing to build on yesterdays knowledge of fetch. Traversing larger ‘messier’ objects and programmatically retrieving values we wanted by passing in data as arguments to functions. I also learnt a lot about diversity in the work place and how we can use to our advantage in solving complex problems. This is because different people have different skill sets, and although sometimes conflict with opposites. We can use each others strengths and not weaknesses to solve problems faster.

### Day 11:

**Today's Progress**: Cognitive Diversity & Continuation of Objects

**Thoughts:** I learnt a lot about diversity in the work place and how we can use to our advantage in solving complex problems. This is because different people have different skill sets, and although sometimes conflict with opposites. We can use each others strengths and not weaknesses to solve problems faster. 

I also continued to build on yesterdays knowledge of fetch. Traversing larger ‘messier’ objects and programmatically retrieving values we wanted by passing in data as arguments to functions.

---
