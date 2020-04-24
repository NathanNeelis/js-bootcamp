<h2>push();</h2>
adds an array item at the end.

<h2>pop();</h2>
removes the last value of the array. also returns the value.

<h2>shift();</h2>
get and remove item from the front of the queue (array);

<h2>unshift();</h2>
adds a array item at the start.


<h2>.indexOf();</h2>
returns the index of a value in the array. So it returns the position of you request in the array.<br/>
<i>console.log("coconut".indexOf("u"));<br/>
// → 5</i>

<h2>.lastIndexOf();</h2>
returns the index of a value in the array counting from the end.

<h2>.slice(x, y);</h2>
Gives you the numbers in between your values from the array. includes starting index and excludes ending index.
Also if you only give one parameter, it counts as a starting position and returns the rest of the array.<br/>
<i>console.log("coconuts".slice(4, 7));<br/>
// → nut</i>

<h2>.concat() </h2>
glues arrays together. Just like the + operator does for 'strings'.

<h2>.trim();</h2>
removes the whitespace. (spaces, newlines, tabs, and similar characters).<br/>
<i>console.log("  okay \n ".trim());<br/>
// → okay<br/></i>

<h2>.padStart(x, "y");</h2>
add a desired length of characters.<br/>
<i>console.log(String(6).padStart(3, "0"));<br/>
// → 006<br/></i>

<h2>.split(); // .join();</h2>
You can split or join values together. example:<br/>
<i>let sentence = "Secretarybirds specialize in stomping";<br/>
let words = sentence.split(" ");<br/>
console.log(words);<br/>
// → ["Secretarybirds", "specialize", "in", "stomping"]<br/>
console.log(words.join(". "));<br/>
// → Secretarybirds. specialize. in. stomping<br/></i>

<h2>.repeat(x);</h2>
You can repeat values.<br/>
<i>console.log("LA".repeat(3));<br/>
// → LALALA<br/></i>


<h2>Rest Parameters</h2>
Accepting any number of arguments by using three dots before the functions last parameter.<br/>
<i>function max(...numbers) {<br/>
  let result = -Infinity;<br/>
  for (let number of numbers) {<br/>
    if (number > result) result = number;<br/>
  }<br/>
  return result;<br/>
}<br/>
console.log(max(4, 1, 9, -2));<br/>
// → 9<br/></i>


<h2>Math objest</h2>
Math.max<br/>
Math.min<br/>
Math.sqrt (square root) - > wortel<br/>
Math.random(); gives a random number between 0 en 1.<br/>
