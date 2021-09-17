
- INTRODUCTION
	- read javascript specification
	- javascript is divided into three core pillars:
		- types:
			- primitive types
			- abstract operations
			- coercion
			- equality
			- TypeScript, Flow etc.
		- scope:
			- nested scope
			- hoisting
			- closure
			- modules
		- objects:
			- this
			- class {}
			- prototypes
			- OO vs. OLOO
- (I)TYPES -- first pillar 
	- primitive types:
		- undefined
		- string
		- number
		- boolean
		- object
		- symbol
	- typeof operator
		- undefined vs. undeclared - starting with the emptiness
		- special values - NaN - which indicates an invalid number
			- NaN is not equal to itself (NaN != Nan)
			- -0 (negative zero)
	- coercion (aka type conversion) - Type coercion is the automatic or implicit conversion of values from one data type to another (such as strings to numbers):
		- abstract operation:
			- ToPrimitive()
			- ToString()
			- ToNumber()
			- ToBoolean()
	- equality(== vs ===)
		- "if you are trying to understand your code, it's critical you learn to think like JS"

```
var student1 = "Frank";
var student2 = `${student1}`;

student1 == student2;            //true
student1 === student2;           //true
```
		- prefers numeric comparison (ToNumber) - string become the number
		- AVOID: 
				- == with 0 or ""(or even "   ")
				- == with non-primitives
				- == true or == false. use ===
		- 
		- if the types are known, == is the best
	- static typing
