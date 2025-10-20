# README #1

## Author: Josiah Shiraki
## Purpose: Documenting the starter labs (Lab 02–05) — what I learned, challenges faced, and what each program is meant to do

# Lab02: Command Line
This lab focused on iterating through the challenge files in a specific order using the Linux command line.

## Challenges
### Getting Used to the Linux Syntax
I had some experience working in the Windows PowerShell terminal from CS 111, but the Linux terminal behaved differently. I had to look at the reference sheet often while learning how its syntax worked.

### Altering Permissions
This was one of the harder parts of the lab. It took me time to understand what the characters meant (for example, rwxrw-r--) and then figure out how to change them correctly using commands like chmod.

# Lab03: C Programming Lab
This challenge was meant to get us used to programming in C, especially with print statements and data types.

## Challenges
### Using the Correct Data Type in printf()
Unlike Python or Java, C requires you to specify the exact data type in each print statement (for example, %d, %f, or %c). I often made small mistakes with this early on, which caused little bugs that were easy to fix but happened often.

## Features
We didn’t create separate functions in this lab. Instead, we wrote all the print statements inside the main function and hardcoded values to produce the required formatted output.

# Lab04: Data Types and Strings
I had an easier time with this lab. Since I’ve been coding since high school, the main challenges were just finding the right C syntax for the logic I already knew.

## Challenges
### Bitmasking
This was the hardest new concept for me. Bitmasking uses bitwise operators to check or manipulate bits in numbers. I had to write out the operations on paper to make sure I understood what was happening and that I was getting the correct output.

## Main Features
### Debugging
In this lab, we were given prewritten functions that didn’t work correctly and had to fix them. Common issues involved incorrect data types and casting problems.

### Writing Simple Functions
I had fun with these functions because they were similar to the problems I did for practice in CS 111 and in my high school classes. It was mostly a matter of using the correct C syntax. Some of the functions we wrote included any_bit_is_one and any_bit_is_zero, which use bitmasking and bitwise operators to determine whether certain bits in an integer are 1 or 0. We also wrote string functions like str_len, which returns the length of a string input, and to_upper, which converts all lowercase letters in a string to uppercase.

# Lab05: Image
This lab was much more challenging. The biggest issue for me was understanding how the pixel data was stored in a one-dimensional array instead of a two-dimensional one (in Python image labs, we used 2D arrays).

## Challenges
### OR Filter
Most of the earlier filters were simple because each pixel was processed once. The OR filter, however, required comparing and combining each pixel with its top and bottom neighbors using the bitwise OR operation. This meant handling edge cases for the first and last rows and using the copy function properly to avoid overwriting data.

## Coded Filters
### OR Filter
Described above — combines pixel values with their top and bottom neighbors using bitwise OR.

### Remove Color Channel
This filter removes a specified color channel (red, green, or blue) by setting all pixel values in that channel to 0.

### Grayscale
Converts the image to grayscale using the formula
Y = 0.299 * R + 0.587 * G + 0.114 * B
and assigns that value to all three color channels.

## Image Outputs
The main function calls each of these filters (the remove color channel function three times, once for each color) and outputs new image files showing the altered versions.

