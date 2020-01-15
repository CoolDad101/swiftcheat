# **SWIFT language notes**


## FILE TOP LEVEL
### import          
module import statements can go top level of a File
### var/let         
global variables can be assigned
### func(){*Executable code goes here*}         
function declarations can be global

## SCOPES
### module
a module is a Scope aka "top level namespace", Frameworks are considered modules(*also are top level namespaces*)
### file
a file is a Scope
### {*methods like to live in here!*}
curly braces are a Scope


## OBJECT TYPES
a type is a set of methods describing what all instances of that type can do (encapsulation of functionality)
### class
### struct
### enum

## NAMESPACES 
### Example:
##### class thisIsMyNamespace {
#####                          class thisIsProtected {*defining this class within another namespace protects it "nested type"*}         
#####                         }

### MESSAGE SENDING BETWEEN NAMESPACES(**see dot notation syntax**):
##### thisIsProtected.thisIsMyNamespace
initiates message sending between these two Classes 'seeing into another scope'

## VARIABLE AND CONSTANT
### var
assign as variable
### let
assign as constant

## MATH OPERATORS
#### +

#### -

#### *

#### /

#### % (remainder)

## COMPARISON OPERATORS

#### == (tests for equivalency, *'equals'*)

#### !=
Not equal

#### <
Less than

#### >
Greater than

## ASSIGNMENT OPERATOR
#### = (**this is for assignment not math**)

## LOGIC OPERATORS
### &
AND
### ||
OR
### !
NOT

## OTHER OPERATORS
### ->
points to the type of return value to be provided by a function ie: -> Int

### \n
creates line break for a string

## DATA TYPES

### Data
Byte buffer

### String
"*words and letters go here...is this a UTF base?*"

### Int
Integer ie. 1...10, U==Unsigned, 8-64 Bit Range

### Integer Variants
Int8: -128 to 127  
Int16: -32768 to 32767  
Int32: -2147483648 to 2147483647  
Int64: -9223372036854775808 to 9223372036854775807  
UInt8: 0 to 255  
UInt16: 0 to 65535  
UInt32: 0 to 4294967295  
UInt64: 0 to 18446744073709551615  

### Float(unsigned)
Decimal Values  
ie. "6345631.432"  

### Float Variants(values determined by .greatestFiniteMagnitude using Darwin, accuracy compiler dependant?)
float: 3.4202823e+38  
float32: 3.402823E+38  
float64: 1.7976931348623e+308  
float80: 1.189731495357231765e+4932  
cfloat: 3.402823e+38  

### Double(unsigned)
64 bit Wide number range Decimal  
ie. "134634563456.001"

### Double Variants(values determined by .greatestFiniteMagnitude using Darwin, accuracy compiler dependant?)
double: 1.7976931348623e+308  
clongdouble: 1.189731495357231765e+4932  
cdouble: 1.797693134862316e+308  

### Bool(these values are literal types and can not be converted to other types in Swift, for clarity and error redduction)
#### TRUE
#### FALSE

## COMMON FUNCTIONS
### print()
print command
default parameters(are interchageable): separator:", ", terminator:"\n"
### return " "
returns specified object
### import
imports Frameworks, Modules. Use at application top level or within desired scope

## CLASS INSTANTIATION
### ()
Use parenthese to instantiate a predefined Object(see **Object**)  
ie: soapbars() an Object "soapbars" is instantiated by calling its name.

## KEYWORDS
### self
ie: self.functionvariablemethod calls an object(functionvariablemethod) within the scope of the instance you are working in.
### private
keeps associated property private to the instance it belongs to, the property will not be seen from outside its instance.
### return
Defines the return value of a function
### inout
function parameter, need further definition


