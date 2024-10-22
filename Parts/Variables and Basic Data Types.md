- Primitive data types works
	- int, double, float, **String** (Capitalized only), char, ...
	- To print them is way simpler than C: System.out.print(variable)
- Also, there are boolean variables in this language by default (differently from C) -> **true** or **false**

### Details
- Double > int (it cant store decimals)
- char = 'a' **NOT** char = "a" -> For single character: ' '
- **STATIC TYPING** -> NOT compiling if a variable is assigned a value of a different type from the declared

#### Strings
- Any sequence of characters between " "
- To create a string:
	- String something = "something";
	- String something = new String("something") -> New String **OBJECT**
- "\" allows to break the sequence and add different things
	- Bytes, different characters, etc
		- " \\\\ " -> " \\ " | " \\" " -> " " "
		  
		  
#### Convention
- Variables can start with just normal alphabetic characters, or `$`, or a `_`, but they are special characters, that serves specific purposes
- Variables are case sensitive
- For readability and convention reasons:
	- Start with lowercase
	- InsteadOfUsingSpace, use capital letters to indicate that "isEven", for example
	- Avoid numbers in general
	- Try to make it objective and simple

---------

## Summary:

Data types:
- **int**, which stores **whole numbers**.
- **double**, which stores **bigger whole numbers** and **decimal numbers**.
- **boolean**, which stores **true** and **false**.
- **char**, which stores **single characters** using **single quotes ( ' ' )**.
- **String**, which stores **multiple characters** using **double quotes ( " ")**.

**Static typing** -> Avoids putting the wrong data type in a certain variable (Better safety).

--------

## Manipulation of variables

- **Addition** -> + and ++ to add 1
- **Subtraction** -> - and -- to subtract 1
- **Multiplication** -> *
- **Division** -> / (If it is dividing a int value, it floors it if there is any floating point in it) 
- **Modulo** -> %
- **Power** -> Math.pow() (we need to import java.lang.Math first )

Operation order:

| Order | Operator                       |
| ----- | ------------------------------ |
| 1     | Parenthesis                    |
| 2     | Exponents                      |
| 3     | Modulo/Multiplication/DIvision |
| 4     | Addition/Subtraction           |


Assignment operators:
- `variable op= value`
- **variable** is an already defined variable with a value in it
- **op** is one of the operations above
- **value** is an valid value for it

-----
## Variable keywords
**final** Keyword -> The variable declared after cannot be manipulated anymore