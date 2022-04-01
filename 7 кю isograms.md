```
Изограмма — это слово, в котором нет повторяющихся букв, последовательных или непоследовательных. Реализуйте функцию, определяющую, является ли строка, содержащая только буквы, изограммой. Предположим, что пустая строка является изограммой. Игнорировать регистр букв. isIsogram("Dermatoglyphics") == true isIsogram("aba") == false isIsogram("moOse") == false // -- игнорировать букву…

```
//An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.
//======= TESTS ========
//isIsogram("Dermatoglyphics") == true
//isIsogram("aba") == false
//isIsogram("moOse") == false // -- ignore letter case
```
function isIsogram(string){
var str = string.toLowerCase().split("").sort().join("").match(/(.)\1+/g);
if(str == null){
return true} else{
return false;
}
}
```