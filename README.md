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

**Today's Progress**: N/A

**Thoughts:** N/A
