# Description
https://www.codewars.com/kata/52fba66badcd10859f00097e/train/javascript
```
Trolls are attacking your comment section!

A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.

Your task is to write a function that takes a string and return a new string with all vowels removed.

For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

Note: for this kata y isn't considered a vowel.
```
Solution 1#
```
function disemvowel(str) {

  var str = str.replace(/a/gi,'').replace(/e/gi,'').replace(/i/gi,'').replace(/o/gi,'').replace(/u/gi,'');

  return str;

}
```

Solution 2# (slightly more concise)
```

function disemvowel(str) {

  return str.replace(/[aeiou]/gi, '');

}
```