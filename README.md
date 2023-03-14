# Typescript is a compiler for Javascript
---

### The command used to make the changes effective on the Js file from ts is
<h3><strong>tsc main.ts -w</strong></h3>

### In the tsconfig.json file, you need to set the rootDir by pointing to the 'src' folder './src', then you move on to set the 'outDir' by pointing to the destination of the compiled files './build/js'

<p> while compiling typescript files we use 'let' to set a variable, however, when watching it using 'es5 under the tsconfig.json file, in the target section, the js file is changed into 'var' to set variables</p>
<p> Using 'es2016 or es6' and later is cool for most recent browsers, however for compatibility with older browsers, 'es5' and below should be your go to</p>

<h2> Deleting a '.ts' file doesn't automatically delete the compiled '.js' file</h2>

<p>It is worthy to note that if you create a file outside the source folder, it will be automatically compiled, to avoide this you need to imput this line of code in the tsconfig.json file ,
  "include": [
    "src"
  ]</p>

### Now the new ts file place outside the src folder is not compiled automatically, and that is the aim.

### let a = 12
### let b = '6'
### let c = 2

### console.log(a / b) {Typescript is not a fan of inference, hence, it figures out that 'a of type int' being divided by 'b of type string' is against it's scripting policy, hence the signal under 'b' however, Js doesn't mind}

## Better put for the compiler's peace of mind
<!-- let a: number = 12
     let b: number = 6
     let c: number = 2 -->

### 'noEmitOnError' is a tsconfig.json settings that is required if you don't want the compiler to compile when an error is observed on the typescript file. 

## Typescript Terminologies

### Typescript is a strongly typed language. It is a statically typed language which means types are checked at compile time.

## <em> Benefits Includes </em>
<ul>
    <li> Self documenting </li>
    <li> Catching Errors during development</li>
    <li> Great for teams</li>
</ul>

### Inplicit and Explicit data type inference by typescript
   let myName = 'Raymond' (hovering the mouse around this suggests it is a string type variable) {string:} Implicit declaration

   let myName: string = 'Raymond' Explicit declaration of the variable type to be a string.

<pre>
 string type data : expects strings 
 number type data : expects numbers {int, float, double
 boolean type data : expects true / false
 union type data : strings | number (these are data that can either be number or strings)
 any type data : expects any type of data amongst the earlier declared
 re type data : regular expression '/\w+/g' where the g stands for global
 </pre>

<pre>
let myName: string = 'Raymond'
let meaningOfLife: number;
let isLoading: boolean;
let album: any;

myName = 'Noela'
meaningOfLife = 28
isLoading = true
album = 1995
</pre>
## Functions
