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