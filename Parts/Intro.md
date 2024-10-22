- **JVM** (Java Virtual Machine) -> One of the big pros about Java
	- Makes the java code run everywhere

- To compile "*javac NameOfTheMainClass.java*"
- To run "*java NameOfTheMainClass*"

---------

Analyzing a Java file.

There is always:
- Class -> A concept part, one section of the code dedicated to execute a certain function -> POO based, so you could call it an object
	- A file will always have one class named after the file
- Method -> Much like python, we have here a "function" of a class, generally it's named "main"
	- public static void main(String[] args) 
	- Just for note, i think, as i am in the beginning and do not know much about Java code:
		- `public` -> Acessible from the outside (by calling it externally)
		- `static` -> Just for scope -> It is accessible in this class only/on this file only
		- `void` -> Does not return anything
		- `String[] args` -> What it works with, or what will be the stdout
			- *"Actually, as the text said here: `String[] args` is a placeholder for information we want to pass into our program"* 
			- So it is just a place holder for not giving the method any arguments
- Statement/Action -> The logic that will happen inside the function

-------

Analyzing the print statement

System -> Built-in class that contains a lot of useful content
out -> Manages the output
println -> Short for printline (ends with "\n" automatically)
- If you want to access the C-like print just put print, without ln
- If you put and println after, it will still print consecutively, but as it ends the line normally you'll just break line after

----------

To comment code (The same as JS):
- `// Comment`
- ```/*
  comment can break lines now
  */```

Javadoc commentings -> Makes the documentation for APIs (Methods, classes, just like """ thing """ in python) 
```/**
* The following class
* That does that and this does this
*/
class thing {}
```


----
Summary:

- Java programs have at least one class and one `main()` method.
    - Each class represents one real-world idea.
    - The `main()` method runs the tasks of the program.
- Comments help the understanding for human readers.
- Java has whitespace, curly braces, and semicolons.
    - **Whitespace** is for humans to read code easily.
    - **Curly** braces mark the scope of a class and method.
    - **Semicolons** mark the end of a statement.
- Java is a compiled language.
    - Compiling catches mistakes in our code.
    - Compilers transform code into an executable class.
