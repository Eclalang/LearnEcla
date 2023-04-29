# How to start

## 1. Create a new project
Create a new file with the extension `.ecla`.

## 2. Run your program
To run your program which is empty for the moment, use the following command `Ecla filename`.  
In our example, you will do : `Ecla .\HowToStart\empty.ecla` and have the following result :  
![img.png](img/empty.png)

## 3. Create a variable

### What is a type ?
A type is a way to define the nature of your variable.
For example, if you want to store a number, you will use the type `int` or `float` depending on the precision you want.  
There is a multitude of types, you will learn them in the next section.

### Different types
First you need to know that several types exist in Ecla for your variables.  
Here is a list of all of them : `bool, float, int, string, list, map`

### Creation
Now that you know the types, we will create our first variable.  
To create it you will always use the same syntax : `var varName type;`.

### Example
In our example, we will create a `string` variable named `str` and some others variables with different types.  
![img.png](img/varCreationError.png)  
If you try to run this program, you will have an error because you didn't use the right syntax.
Something important to know, like in others languages (C, Java or JavaScript) you need to finish your line by `;`.  
The purpose of this is to announce the end of line.  
To fix it, you will have to add a `;` at the end of your first line and specify that `num` is a variable like this :  
![img.png](img/varCreation.png)  
If you try to run this program : `Ecla .\HowToStart\varCreation.ecla`.  
You will have the same result as previously because our variables don't have a value assigned.

## 4. Assign a value to a variable

### Assign a value
Now that you know how to create a variable, you will have to assign a value to it.
Then to define a value to your variable, you will use : `varName = value;`  
You can also define the variable with its value directly with : `var varName type = value;`

### Example
In our example, we will assign a text to our variable `str` and a number to our variable `nb`.  
![img.png](img/varAssign.png)  
If you try to run this program : `Ecla .\HowToStart\varAssign.ecla`.  
You will have the same result as previously because our variables are still not printed.

## 5. Print
Until now, you learned how to create a variable and assign a value to it. But you can't see the progression of your program.  
So what we are going to do is print the value of our variable.  
To print in Ecla you will have to use one of our standard library, console.

### Import a library
To start, you will have to import the library by using the keyword `import` followed by the library name.  
So in our case to import the library console, you will write : `import console;`.

### Use a library
Now that our library is imported in our code, we will be able to use it.  
To use a function from a library, you will use the following syntax : `libraryName.functionName();`

### Example
Here we want to print our variable `str`. To do so we will use the function `print` from the library console.  
![img.png](img/print.png)  
If you execute the program `print.ecla`, it will print the value of the variable str in your terminal like this :  
![img.png](img/printresult.png)  
Well done you did your first Hello, World! in Ecla!  
_Here we printed the value of a variable, but you can also print a value directly._

## 6. Create your first function

### What is a function ?
A function is a block of code where multiple instructions are grouped together.  
It can be called as many times as you want from anywhere in your program.

### Creation
Now you know how to create a variable and use a library to print it.
Let's advance to the next step and create a function.
For this you will need a new keyword `function`.  
To create your function, you will use this syntax : `function functionName() {}`. Then you write your code between the braces.

### Call
If you just create your function and execute your program, it won't print anything because the code in your function
is never executed because your function is never called.  
So to call your function, you simply write the name of your function `functionName();`.

### Example
We will reuse our previous code but put in a function named `hello` and called it like this :  
![img.png](img/hello.png)  
It will give you the same result as before.  
If you call your function multiple times, it will print the same value multiple times. Here I called it 2 times :  
![img.png](img/MultipleHello.png)  
And I ended up with 2 times the same value printed.

## 7. Function parameters
You learned how to create and call a function but if you want to change the value printed, you will have to change the function itself.  
Instead you can use parameters for your function to print whichever value you want.  
To make your function takes one or more parameters, you will define it between the parenthesis `functionName(varName : varType, var2Name : var2Type) {}`.

### Example
For this example we will add 2 `string` parameters to our function hello then print the 2 values.  
You can see bellow the program and the result expected :  
![img.png](img/parameters.png) ![img.png](img/parametersresult.png)

## 8. Return a value

### Return a value from a function
Until now our function was used to print a string but what about creating a function to add a number to another one ?  
So instead of printing, you will return your value using the keyword `return`.  
At first, you need to define the type you want to return from your function after your parameters' parenthesis,
you need to open new parenthesis where your precise the type returned like this : `funcName(var : type) (int) {}`.  
Secondly, at the end of your function you put your return followed by the value wanted like this : `return value;`.

### Example
We create a function add which takes 2 int parameters and return the addition of both (in this case an int).  
Then in another function main, you define 2 variables, call the function add with this 2 variables and print the result.  
![img.png](img/return.png) ![img.png](img/returnresult.png)

## 9. Conditions

### If
