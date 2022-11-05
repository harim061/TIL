# 2. Strings

## 2-1. Strings
> you can create a string in JS by using the double quotes " or single quotes '

### String property
*.length* - used to return the length of the string

### String methods
*.toLowerCase()* - return a new string that has all of its characters in lower case

🔸 .length shold not have () after it -> property 

🔸 .toLowerCase() requires () -> method, it's an  action that you are performing

*.toUpperCase()* - return a new string in upper case
 
 ## 2-2. Character access
 > you can access a specific character in a string by using []
 > 
 > you have to provide the index of the character that you'd like to access, starting from 0

### Combining it with length
```
const language = "JavaScript";
language[ language.length - 2 ]; //p

language[language.lenth] //undefined
```

### .at(index) method
```
const language = "JavaScript";
language.at(0); // "J";
language.at(-2); // "p";
language[-1] //undefined
```
🔸 .at() methond is for negative indices

### JSDoc
```
/**
 * @param {string} name
 */
 ```
 
 ## 2.3 Substrings
 > is a part or a portion of a string
 
 ex) "rain" is a substring of the string "brain" because you can get "rain" by taking the last 4 characters
 - often need to get a few characters of a string rather than all of it. we use the substring method

### Substring signature
```
someString.substring(indexStart,indexEnd)
```
- indexStart : the position of the first character you'd like to include
- indexEnd : the position of the first character you'd like to ignore
  - optional parameters : you can pass the indexStart and it'll assume the indexEnd to be the same as the string length

## 2.4 Plus operator
> will behave differently based on the types of values you use it with
> 
> merging 2 strings together into 1 string

```
"hello"+"world" //hello world
```
### += opertaor
```
let name = "noh";
name = name + "harim";
console.log(name); //"noh harim"
==
let name = "noh";
name += "harim";
console.log(name); //"noh harim"
```

## 2.5 Template strings
> template strings support interpolation and other nifty features

```
`This is a template string`
```
- only difference is that template strings start and end with a backtick ` 
- template strings can span multiple lines

### Interpolation
> you could write a variable in your string and get its value
> wrap your variable name with a dollar sign and curly braces
```
let lan = "javascript";
`I am learning ${lan}`;
```

 💥nutrition tabl
 ```
 return
    `<tr>
    <td>${label}</td>
    <td>${value}</td>
    </tr>`;
 ```
 ![image](https://user-images.githubusercontent.com/90364684/200104345-8b56c70d-2e6e-4523-bb31-cfcf0506585a.png)
