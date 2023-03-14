# Typescript is a compiler for Javascript
---

### The command used to make the changes effective on the Js file from ts is
<h3><strong>tsc main.ts -w</strong></h3>

### In the tsconfig.json file, you need to set the rootDir by pointing to the 'src' folder './src', then you move on to set the 'outDir' by pointing to the destination of the compiled files './build/js'

<p> while compiling typescript files we use 'let' to set a variable, however, when watching it using 'es5 under the tsconfig.json file, in the target section, the js file is changed into 'var' to set variables</p>
### Using 'es2016 or es6' and later is cool for most recent browsers, however for compatibility with older browsers, 'es5' and below should be your go to</p>

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

## 'noEmitOnError' is a tsconfig.json settings that is required if you don't want the compiler to compile when an error is observed on the typescript file. 

## Typescript Terminologies

### Typescript is a strongly typed language. It is a statically typed language which means types are checked at compile time.

## Benefits Includes
<ul>
    <li> Self documenting </li>
    <li> Catching Errors during development</li>
    <li> Great for teams</li>
</ul>