---
language: KSP
filename: 
contributors:
    - ["Cameron Hansen", "github.com/cambo2015"]
---

KSP stands for Kontakt Script Processor
It is a scripting language that is developed by Native Instruments, and is used to make virtual instrument plugins. KSP Scripts runs inside the full version of the Kontakt Player. 


```ksp
{Comments go inside brackets}
 {This is a comment}

{show message}
message("Hello world!")

{TYPES}
{int}
10

{real number (float)}
10.0

{string}
"some text"


{VARIABLES}
{Create a variable}
declare $x
{Assign 10 to a x}
$x := 10

{ You can also do}
declare $y := 10
declare $sum := $x +$y

{string variable}
declare @mystr := "some text"




{MATH}

{Equals 5}
10/2
{Equals 30}
6*5
{Equals 20}
15+5
{Equals 7}
5+2
{Equals 1}
5 mod 2 
{negative value}
-10
{Equals 10}
abs(-10)
{increment by 1. Equals 11}
inc(10)
{decrement by 1. Equals 9}
dec(10)
{random number)
$rand = random($min,$max)

{CASTING}
{int to float. Equals 10.0}
int_to_real(10)

{float to int. Equals 10}
real_to_int(10.0)

{BOOLEAN OPERATORS}
{greater than}
$x > $y
{less than}
$x < $y
{greater than or equal}
$x >= $y
{less than or equal}
$x <= $y
{equal to}
$x = $y
{not equal to}
$x # $y
{ true if z exists in a range between x and y}
in_range(z,x,y)
{true if x is false}
not $x
{true if both are true}
$x and $y
{true if one is true}
$x or $y

{LOGIC}
if($x = $y)
  $x := 2
if($x # $y)
  $x := 50
else
  $x := 200
end if


{FUNCTIONS}
{create a function}
function myFunc
  message("hello world")
{call a function}
call myFunc

