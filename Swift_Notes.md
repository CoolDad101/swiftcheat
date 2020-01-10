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

## DATA TYPES
### String
"*words and letters go here...is this a UTF base?*"

### Int
Integer ie. 1...10, U==Unsigned, 8-64 Bit Range

### Integer Variants
Int8
Int16
Int32
Int64
UInt8
UInt16
UInt32
UInt64

### Float
Decimal Values 1.001, 32 bit

### Double
Wide number range + Decimal  100000000.001, 64 bit

### Bool
#### TRUE
#### FALSE

## COMMON FUNCTIONS
### print()
Print command
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


