
<h3> Binding visibility: Lexical scoping </h3>
<p> The set of bindings visible inside a block is determined by the place of that block in the program text. Each local scope can also see all the local scopes that contain it, and all scopes can see the global scope. <p>
  
  <h3> Arrow functions </h3>
  <p> The arrow functions is made of "=>". The arrow comes after the list of parameters and is followed by the function’s body. It expresses something like “this input (the parameters) produces this result (the body)”.When there is only one parameter name, you can omit the parentheses around the parameter list. If the body is a single expression, rather than a block in braces, that expression will be returned from the function. So, these two definitions of square do the same thing:
  <br/> <br/>
<i>
const square1 = (x) => { return x * x; }; <br/>
const square2 = x => x * x; <br/>
  </i> 
   <br/>
When an arrow function has no parameters at all, its parameter list is just an empty set of parentheses. <br/>
 <br/>
const horn = () => { <br/>
  console.log("Toot"); <br/>
}; <br/>

</p>

<h3> Methods </h3>
<p> <b> forEach </b> <br/>
  works similar to a for/of loop as a higher order function <br/>
  Example: <br/>
  <i> ["A", "B"].forEach(l => console.log(l)); <br/>
// → A <br/>
// → B <br/>
  </i>
   <br/> <br/>
  <b> Filter </b> <br/>
  A filter functions writes a new array with the filtered results. So it does not delete the other items in the original array. <br/>
  It looks like this: <br/>
  <i> console.log(SCRIPTS.filter(s => s.direction == "ttb")); <br/>
    // → [{name: "Mongolian", …}, …] </i> <br/>
   <br/>
  It works like this: <i><br/>
  function filter(array, test) {<br/>
  let passed = [];<br/>
  for (let element of array) {<br/>
    if (test(element)) {<br/>
      passed.push(element);<br/>
    }<br/>
  }<br/>
  return passed;<br/>
}<br/>
<br/>
console.log(filter(SCRIPTS, script => script.living));<br/>
// → [{name: "Adlam", …}, …]<br/>
  </i> <br/>
  <br/>
  <b> Map </b><br/>
  So the mapping methods creates once again a new array. This array has the same length of the old one but...<br/>
  its content will have been mapped to a new form by the function.
 <br/><br/>
  It looks like this:<br/> <i>
  let rtlScripts = SCRIPTS.filter(s => s.direction == "rtl");<br/>
console.log(map(rtlScripts, s => s.name)); // this is the map method call.<br/>
// → ["Adlam", "Arabic", "Imperial Aramaic", …]<br/>
  </i><br/>
  It works like this:<br/><i>
  function map(array, transform) {<br/>
  let mapped = [];<br/>
  for (let element of array) {<br/>
    mapped.push(transform(element));<br/>
  }<br/>
  return mapped;<br/>
}</i><br/>
  
  
  
