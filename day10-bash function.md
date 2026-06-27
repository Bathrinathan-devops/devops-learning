## Day 10 - function in bash

### what is function?
A function  is a reusable block of code.
write once - use many times
saves times and make code cleaner

### Function Structure:
## Part 1- Define the function :
Functiononname() {
 echo "do something"
 }
 like writting a srecipe in cook book , nothing happens yet - just saved!

 ## part 2 - call the function:
 functiononname "argument"
 now it actually runs
 can call as many times as you want

 ### Function with Arguments:
 greet() {
 echo "hello $1!"
 echo "welcome $2!"
 }
 greet "Bathrinathan" "to DevOps"

 ### Argument variables:
 check_server() {
    echo "checking server $1..."
    echo "Status: Running!"
    echo "---------------------"
    }
  check_server "web"
  check-server "Database"
  check_server "backup"

  ### Naming rules:
  -Use lower case
  -Use underscore for spaces
  -check name descritive
  -check_server not cs
  -Define and call mist EXACTLY!

  My understading 1:
  Function name is our choice based on requirement 

  greet() - our choice 
  check_server() - our choice
  battery_check - our choice

  My understading 2
  "when multiple students i can call function multiple time
   student "Bathrinathan" "chennai" "Devops"
   student "Raj" "membai" "cloud"
   student "priya" "Bangalore" "SRE"

   my understand 3
   $1 is first argument , $2 is second argument

   myfunction "hello"  "world"
                $1         $2

      Golden Rules to remember:
      1. Define first - then call
      2. Name must match exactly
      3.$1 $2 $3 for arguments
      4.{ } holds function code
      5. call as many times as needed!
