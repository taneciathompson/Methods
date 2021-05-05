Strings

Methods,their meanings, examples, and time complexities

charAt()- 
Returns character at specified index in a string. Index of the first character is 0, the second is 1 and so on.

ex.
Phrases
var str= "That's all Folks!"
var res = str.charAt(str.length -1)
console.log(res)

expected result- "!"

var str = "How you doing?"
var res = str.charAt(0)
console.log(res)

expected result- "H"


var str = "What you talking bout Willis?"
var res = str.charAt(7)
console.log(res)

expected result- "u"

Time Complexity- O(1)

charCodeAt()-
Returns the unicode of the character at the specified index in a string. Index starts at 0.

ex-
Song Lyrics

var str = "Wake me up before you go-go!"
var  b = str.charCodeAt(0)
console.log(b)

expected result-  87

var str = "For the world is full of zanies and fools, who dont believe in sensible rules"
var c = str.charCodeAt(20)
console.log(c)

expected result- 108

var str = "Cotton candy, sweet and low, let me see you tootsie roll!"
var tr= str.charCodeAt(27)
console.log(tr)

expected results- 44
Time Complexity- O(1)

Concat()-
is used to join two or more strings does not change existing strings, returns a new string containing text of joined strings.

ex-
Song Titles

var str1 = "Ante"
var str2 = "Up!"
var res = str1.concat(str2)
console.log(res)

expected result- "AnteUp!"

var str1= "Like"
var str2 = "You"
var res = str1.concat(str2)
console.log(res)

expected result - "LikeYou"

var str1 = "Baby"
var str2 = "Boy
var res= str1.concat(str2)
console.log(res)

expected result- "BabyBoy"


Time Complexity- O(n) if not equal O(n+m)

Includes()-
determines whether a string contains the characters of a specified string. Returns true if it does include the character, false if not.

ex-
Famous People

var str= "George Stephanopoulos"
var g = str.includes("George")
console.log(g)

expected result- true


var str= "Khalid Khalid"
var k= str.includes("steve")
console.log(k)

expected result- false

var str= "Kim Kardashian West"
var w= str.includes("dash")
console.log(w)

expected result- true

Time Complexity- O(n)

indexOf()-
Returns the position of  the first occurance of a specified value in a string. Returns w-1 if the value of the search never occurs.

ex-
Quotes

var str= "I have a dream!"
var m = str.indexOf("dream")
console.log(m)

expected result- 9

var str= "I've been to the mountain top!"
var l = str.indexOf("mountain")
console.log(l)

expected result- 17

var str = "Injustice anywhere is a threat to justice everywhere!"
var k = str.indexOf("threat")
console.log(k)

expected result- 24

Time Complexity- O(n)

Match()-
searches a string for a match against a regular expression, returns the matches, as an array object.

ex-

Dr.Suess phrases

var str= "Today you are you! That's truer than true! There's no one alive more you-er than you!"
var res = str.match(/you/g)
console.log(res)

expected result- 
[ 'you', 'you', 'you', 'you' ]

var str= "I speak for the trees, for the trees have no tongues"
var res= str.match(/tree/g)
console.log(res)

expected result- 
[ 'tree', 'tree' ]

var str= "The more things you read, the more things you will know. The more you learn, the more places you will go!"
var res= str.match(/more/g)
console.log(res)

expected result- [ 'more', 'more', 'more', 'more' ]

Time Complexity- O(n)

Repeat()-
returns a new string with a specified number of copies of the string it was called on.

ex-
Beyonce songs
 var str= "Single Ladies"
 console.log(str.repeat(2))
 
 expected result- Single LadiesSingle Ladies
 
 var str= "Pretty Hurts" 
 console.log(str.repeat(4))
  
  expected result- Pretty HurtsPretty HurtsPretty HurtsPretty Hurts
  
  var str= "Sorry"
  str.repeat(6)
  console.log(str.repeat(6))
  
  expected result-SorrySorrySorrySorrySorrySorry
  
Time Complexity- O(N^2)

Replace()-
searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced

ex-
Song Titles
var str= "Who let the dogs out?"
var res= str.replace("dogs", "cats")
console.log(res)

expected result- "Who let the cats out?"

var str = "I see fire and I see rain"
var res= str.replace("fire", "clouds")
console.log(res)

expected result- "I see clouds and i see rain"

var str = "Where da party at?"
var res = str.replace("party", "shindig")
console.log(res)

expected result- "Where da shindig at?"

Time Complexity- O(n)

Search()-
seraches a string for a specified value, returns the position of the match. the search value can be string or a regular expression. Returns -1 if no match is found.

ex-
Places

var str= "visit winchester"
var n = str.search("maine")
console.log (n)

expected result- -1

var str = "Welcome to Boston"
var m= str.search("Boston")
console.log(m)


var str= "You're in Tallahassee"
var t= str.search "tallahassee"
console.log(n)

expected result- -1

Time Complexity- O(n)

Slice()-
extracts parts if a string and returns the extracted parts in a new string. Use the start and end parameters to specify the part of the string you want to extract.

ex-
Greetings

var str= "Hey ya'll hey!"
var res= str.slice(0,5)
console.log(res)

expected result- Hey y


var str = "Good Evening"
var res = str.slice(3,5)
console.log(res)

expected result- d

var str= "Hello!"
var res = str.slice(2)
console.log(res)

expected result- llo!

Time Complexity- O(1)

Split()-
used to split a string into an array of substrings and returns a new array.

ex-
Questions

var str= "How are you today?"
var res = str.split("")
console.log(res)

expected request- [ 'H',
  'o',
  'w',
  ' ',
  'a',
  'r',
  'e',
  ' ',
  'y',
  'o',
  'u',
  ' ',
  't',
  'o',
  'd',
  'a',
  'y',
  '?' ]
  
  var str= "What's the weather?"
  var res= str.split("")
  console.log(res)
  
  expected request- [ 'W',
  'h',
  'a',
  't',
  '\'',
  's',
  ' ',
  't',
  'h',
  'e',
  ' ',
  'w',
  'e',
  'a',
  't',
  'h',
  'e',
  'r',
  '?' ]
  
  var str= "Where have you been?"
  var res= str.split("")
  console.log(res)
  
  expected results- [ 'W',
  'h',
  'e',
  'r',
  'e',
  ' ',
  'h',
  'a',
  'v',
  'e',
  ' ',
  'y',
  'o',
  'u',
  ' ',
  'b',
  'e',
  'e',
  'n',
  '?' ]
  

Time Complexity- O(len)

Substr()-
extracts parts of a string, beginning at the character at the specified position, and returns the specified numbers of characters.

ex-
Kid Show Characters

var str= "Baby Bop"
var res= str.substr(1,4)
console.log(res)

expected results- aby 

var str= "Lamb Chop"
var res= str.substr(2,4)
console.log(res)

expected results- mb C

var str= "Blue's Clues"
var res= str.substr(6, 9)
console.log(res)

expected results- Clues

Time Complexity- O(1)


toLowerCase()-
Converts a string to lowercase letters

ex-
Full Names

var str= "Tanecia Thompson"
var res= str.toLowerCase()
console.log(res)

expected result- tanecia thompson

var str= "TuckerJames Thompson"
var res= str.toLowerCase()
console.log(res)

expected result- tuckerjames thompson

var str= "Oprah Winfrey"
var res= str.toLowerCase()
console.log(res)

expected result- oprah winfrey


Time Complexity-O(N)

toUpperCase()-
Converts a string to uppercase letters.

ex-
My Favorite Celebrities

var str= "dolly parton"
var res= str.toUpperCase()
console.log(res)

expected result- DOLLY PARTON

var str= "beyonce giselle knowles carter"
var res= str.toUpperCase()
console.log(res)

expected result- BEYONCE GISELLE KNOWLES CARTER 

var str= "tina turner"
var res= str.toUpperCase()
console.log(res)

expected outcome- TINA TURNER

Time Complexity- O(n)

Trim()-
Removes white space from both sides of a string.

ex-
Breakfast

var str= "    eggs   and   bacon   "
console.log(str.trim())

expected results- 
eggs   and   bacon

var str= "     omlettes    "
console.log(str.trim())

expected result- "omlettes"

var str= "     orange juice"
console.log(str.trim())

expected result- "orange juice"


Time Complexity- O(n)
