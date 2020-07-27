# what-i-learned-week-10

## objectify-yourself

* Set the values of new property in object's.

ex.)
// Set the value of property `objectify` to be "yourself".
myCodeImmersivesObj.objectify = 'yourself';

// Add the new property `isAnExcellentObject` and set it to `true`.
myCodeImmersivesObj.isExcellentObject = 'true'



## Objectively Funcy

* Functions and objects together.
* Write function that can manipulate the object passed in.

ex.)
const getFirstName = function(person){
  return person.firstName;
}

const getLastName = function(person){
  return person.lastName;
}


## new-dinosaurs-yay-question-mark

* Given a species name, a period, and a diet, returns a dinosaur object with those values.
* Does not mutate the original object.

ex.)
const makeDino = function(species, period, carnivore, extinct = false) {
const dino = {
  species: species,
  period: period,
  carnivore: carnivore,
  extinct: extinct,
}
return dino
}

## JSON Born

* `getStudentByIndex` - given an index, returns the student with that index from the students array in the `students.json` file
* `getStudentByName` - given a first name, returns the student with that name from the students array in the `students.json` file, and returns -1 if they're not found
* `graduateStudent` - given a student's name, up their term by 1 and write it back to the `json` file

ex.)
const fs = require('fs');
const file = fs.readFileSync('../students.json', 'utf8')

const obj = JSON.parse(file);
//console.log(obj.students)

const getStudentByIndex = function(index){
return obj.students[index]
}


