Strings

Methods,their meanings, examples, and time complexities

charAt()- 
Returns character at specified index in a string. Index of the first character is 0, the second is 1 and so on.

ex.

Time Complexity- O(1)

charCodeAt()-
Returns the unicode of the character at the specified index in a string. Index starts at 0.

ex-

Time Complexity- O(1)

Concat()-
is used to join two or more strings does not change existing strings, returns a new string containing text of joined strings.

ex-

Time Complexity- O(n) if not equal O(n+m)

Includes()-
determines whether a string contains the characters of a specified string. Returns true if it does include the character, false if not.

ex-

Time Complexity- O(n)

indexOf()-
Returns the position of  the first occurance of a specified value in a string. Returns w-1 if the value of the search never occurs.

ex-

Time Complexity- O(n)

Match()-
searches a string for a match against a regular expression, returns the matches, as an array object.

ex-

Time Complexity- O(n)

Reapeat()-
returns a new string with a specified number of copies of the string it was called on.

ex-

Time Complexity- O(N^2)

Replace()-
searches a string for a specified value, or a regular expression, and returns a new string where the specified values are replaced

ex-

Time Complexity- O(n)

Search()-
seraches a string for a specified value, returns the position of the match. the search value can be string or a regular expression. Returns -1 if no match is found.

ex-


Time Complexity- O(n)

Slice()-
extracts parts if a string and returns the extracted parts in a new string. Use the start and end parameters to specify the part of the string you want to extract.

ex-


Time Complexity- O(1)

Split()-
used to split a string into an array of substrings and returns a new array.

ex-


Time Complexity- O(len)

Substr()-
extracts parts of a string, beginning at the character at the specified position, and returns the specified numbers of characters.

ex-

Time Complexity- O(1)


toLowerCase()-
Converts a string to lowercase letters

ex-

Time Complexity-O(N)

toUpperCase()-
Converts a string to uppercase letters.

ex-


Time Complexity- O(n)

Trim()-
Removes white space from both sides of a string.

ex-

Time Complexity- O(n)
