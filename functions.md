
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

