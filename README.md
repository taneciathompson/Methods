# Methods

Arrays


Methods,their meanings, examples, and time complexities

Map()-
an object that holds key value pairs and remembers the original insertion order of keys.


ex.-
Multiply Values by 10
let numbers= [7, 27, 30, 11];
let newArray = numbers.map(newFunction)
function newFunction(num){
return num * 10
}

Expected Result: 70, 270, 300, 110


Get SuperHero Real Identities

let names = [ {firstName: Bruce lastname: Wayne;}, {firstname: Aruthur lastname: Curry}, {firstname: Clark lastname: Kent}, {firstname:Diana lastname: Prince}]
function findName(names){
  let government =[names.firstname,names.lastname].join("")
  return government
}
function findIt(){
   console.log (names.map(government));
}

Expected result: Bruce Wayne, Arthur Curry, Clark Kent, Diana Prince


Find the Square Root


var numbers = [20, ,16 62, 90];
var s = numbers.map(Math.sqrt)
console.log (s);

Expected result: 4.47, 4, 7.9, 9.5

Time Complexity- O(n)


Reduce() -
Reduces an array to a single value, executes a providede function for each value of the array(left to right), returns the value of the function in an accumulator(result/total)

ex- 
Find Sum
const array = [7, 27, 6, 2];
const reducer = (accumulator, currentValue) => accumulator + currentValue;
console.log(array.reduce(reducer))
expected result- 42

Rounded Numbers
var intergers = [14.5, 6.5, 20.4, 18.5]
function add(total,num){
retun total+Math.round(num)
}
console.log(intergers.reduce(add,0))

expected result- 61

Info
let info = [
  { name: 'Joshua', age: 31 },
  { name: 'Thaddeus', age: 20 },
  { name: 'George', age: 20 }
];

function groupBy(objectArray, property) {
  return objectArray.reduce(function (acc, obj) {
    let key = obj[property]
    if (!acc[key]) {
      acc[key] = []
    }
  })  
}     
console.log(info)

expected result- [ { name: 'Joshua', age: 21 },
  { name: 'Thaddeus', age: 20 },
  { name: 'George', age: 20 } ]

Time Complexity- O(n)

Filter()- 
creates an array filled with all  array elements that pass a test

ex-
Find Odd
var oddNum = [3,4,6,7,9,20]
function findOdd(num){
return num % 3
}
console.log(oddNum.filter(findOdd))
expected result- [ 4, 7, 20 ]

Name length
const name = ["Taj", "Tucker", "Taavia","Tanecia", "Tyrone", "Tia"]
const outcome = names.filter(name => name.length < 6)
console.log(outcome)

expected result- ["Tanecia"]

Find Prime
const list = [-4, -7, -3, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13];

function prime(num) {
  for (let i = 4; num > i; i++) {
    if (num % i == 0) {
      return false;
    }
  }
  return num > 1;
}

console.log(list.filter(prime))
expected result- [2, 3, 5, 7, 11, 13]


Time Complexity- O(n)

forEach()-
calls a function once for each element in an array in order.

ex.
Find Total
var totals = [65.00, 44.00, 12.00, 4.00];
totals.forEach(myFunction)

function myFunction(item, index, arr) {
  arr[index] = item * 10;
}
console.log(totals)

expected results- [ 650, 440, 120, 40 ]

Add
var addItUp = 0;
var nums = [90, 47, 62, 88];
nums.forEach(findSum);

function findSum(nums) {
  addItUp += nums;
}
console.log(addItUp)

expected results- 287

List Similar

const inCommon = ['books', 'library', 'school'];

inCommon.forEach(element => console.log(element))

expected result- Books
                 Library
                 School

Time Complexity-O(n)

Sort()-
sorts the time of an array, order can either be alphabetical, numerical, up or down

ex.
Count Points
var points = [80,25,60,10]
points.sort(function(a,b){return a-b})
console.log(points)

expected result- [ 10, 25, 60, 80 ]

Alphabetical Fruit
var fruit = ["orange", "dragonfruit", "nectarine", "fig"]
console.log(fruit.sort)

expected result- [ 'dragonfruit', 'fig', 'nectarine', 'orange' ]

Calender Order
const calender = ['April', 'August', 'October', 'June'];
calender.sort();
console.log(calender);

expected result-[ 'April', 'August', 'June', 'October' ]

Time Complexity- O(n log (n))

Slice()-
returns the selected elements in an array as a new array object. Selects the elements srarting at the given start argument.

ex.
Zoo Slice
const zoo = ['orangutan', 'giraffe', 'lion', 'panda', 'zebra'];

console.log(zoo.slice(2,4))

expected result- Lion, Panda

Find The Best Harry Potter book
const volumes = ['Half-Blood Prince', 'Prisoner of Azkaban', 'Order of Pheonix', 'Philosophers Stone', 'Chamber of Secrets']
console.log(volumes.slice(0,3))

expected result- [ 'Half-Blood Prince',
  'Prisoner of Azkaban',
  'Order of Pheonix' ]
  
Dogs
const pups = ['bulldog', 'boxer', 'poodle', 'puggle', 'great dane']
console.log(pups.slice(-3, -1))

expected result- [ 'poodle', 'puggle' ]

Time Complexity- O(n)


Pop()-
removes the last elemnt of an array and returns that element.

ex-
Soap
var soap = ['dove','irish spring', 'suave', 'pert']
console.log(soap.pop())

expected result- pert

Soda
var cola= ['sprite', 'fanta', 'root beer', 'pepsi']
console.log(cola.pop())

expected result- pepsi

Sea Life
var aquarium = ['shark', 'swordfish', 'octopus', 'seahorse'];

var popped = aquarium.pop();

console.log(aquarium)
expected result-['shark', 'swordfish', 'octopus' ]

console.log(popped)
expected result -'seahorse'

Time Complexity- O(1)

Shift()-
removes the first item of the array

ex.
Cereal
var cereal =["frosted flakes", "cheerios", "cap'n crunch", "applejax"]
var shifted = cereal.shift()
console.log(cereal)
console.log(shifted)

expected results- [ 'cheerios', 'cap\'n crunch', 'applejax' ]
frosted flakes

Tv Dads
   var tele = ["michael kyle", "phil dunphey", "homer simpson", "carl winslow"]
   var shifted = tele.shift()
   console.log(tele)
   console.log(shifted)
   expected result- ["phil dunphey", "homer simpson","carl winslow"]
   "michael kyle"
   
   Best Sport
   var sport=['football','tennis', 'soccer', 'polo', 'lacrosse']
   var shifted = sport.shift()
   console.log(sport)
   console.log(shifted)
   expected result- ['tennis', 'soccer', 'polo', 'lacrosse']
   'football'
   
Time Complexity- O(n)

Push()-
adds new items to the end of an array and returns the new length

ex.
Sneakers
var sneakers = ["nike", "puma", "reebok", "adidas"]
console.log(sneakers.push("new balance"))

expected result - ["nike", "puma", "reebok", "adidas", "new balance"]

Flowers
var species = ['tulip', 'rose','orchid', 'daisies']
console.log(species.push('sunflower'))

expected result- ['tulip', 'rose', 'orchid', 'daisies', 'sunflower']

Snacks
var snacks = ["chips", "honeybuns", "zebracakes", "sour straws"]
console.log(snacks.push("dunkaroos"))

expected result- ["chips", "honeybuns","zebracakes", "sour straws", "dunkaroos"]

Time Complexity- O(1)

unShift()-
adds new items to the beginning of an array of an array, and returns the new length

ex-
Tools
var tools = ["wrench", "hammer", "screwdriver", "monkey wrench"]
console.log(tools.unshift("pliers", "drill"))

expected result- 6

Cars
var vehicles =["jeep", "mercedes", "bmw", "lexus"]
console.log(vehicles.unshift("toyota", "volvo", "chevrolet"))

expected result- 7

Juice
var quenchers = ["apple juice", "orange juice", "cranberry juice",]
console.log(quenchers.unshift("pineapple juice", "grape juice"))

expected result- 5

Time Complexity- O(n)

Includes()-
determines whether an array contains a specified element, returns true if array contains the element and false if not

ex-
Toys

var toys = ["ball", "jumprope", "doll", "puzzle"]
var q = toys.includes("puzzle")
console.log(q)

expected results- true

Reality Shows
var trashTV = ["real world", "real housewives", "bad girls club", "love and hip hop"]
var w = trashTV.includes("black ink")
console.log(w)

expected result - false

Amphibians
var reptile = ["frogs", "salamanders", "caecilians","newt"]
var r = reptiles.includes("newt")
console.log(r)

expected result- true



Time Complexity- O(n)

indexOf()-
searches the array for the specified item and returns its position, starts search at the specified position, or at the beginning if no start is specfied. Ends the search at the end of the array. returns -1 if the item is not found. If the item is present more than once, indexOf method returns the position of the first occurance.

ex.
Colors
var colors = ["purple", "blue", "green", "red", "red", "orange","orange"]
var c = colors.indexOf("orange', 5)
console.log(c)

expected result- 5

Gems
var shiny = ["amethyst", "jade","jade","sapphire", "amber", "ruby", "ruby"]
var s= shiny.indexOf("ruby", 8)
console.log(s)

expected result- -1

WildLife
var wild =["moose", "deer", "rabbits", "deer", "elk"]
var x = wild.indexOf("deer", 2)
console.log(x)

expected results- 3

Time Complexity- O(n)

Every()-
checks if all elements in an array pass a test(provided as a function)
executes a function once for each element present in the array-
if it finds an array element where the function returns a false value, every() returns false(doesn't check the remaining values)
if no false occurs, every() returns true

ex-
Legal Age
var ages = [ 7, 27, 30, 90]
function legal(age){
return age >= 21
}
console.log(ages.every(legal))

expected result- false

Poll
var survey = [
  { name: "Dashlin", answer: "Yes"},
  { name: "Asianna", answer: "Yes"},
  { name: "Julie", answer: "Yes"},
  { name: "Wade", answer: "No"}
];

function same(el, index, arr) {
  if (index === 0){
    return true;
  } else {
    return (el.answer === arr[index - 1].answer);
  }
}
console.log(survey.every(same))

expected result- false

Baby ages
var ages = [24mo, 18mo, 12mo, 48mo];

function infant(age) {
  return age => 18
}
console.log(ages.every(infant))

expected result- true

Time Complexity- O(n)
