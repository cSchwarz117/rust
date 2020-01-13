# Rust HW 1

## Overview

This application is used to calculate the modulous of an exponent. It takes three command line arguments the number, its power and the divosor. It returns the remainer.

## How to Develop

Run the application:

1. Unzip the file`
2. Navigate to the unzipped folder in your terminal
3. Run the application with 3 U32 integer arguments: `cargo run 2 2 2`


## How to Test

1. Run `cargo test` in command line

## Writeup

For this program I took most of the format from the GCD example in chapter 2 then reworked it to create a working command line program. I considered some issues with trying to test the program based on command line arguments and realized I would need to do my assert!() within the modexp function and not before main passed the arguments into modexp. My test simply check that the integers do not overflow the U32 variables and check that some simple inputs produce correct results.

One issue I seemed to not be able to solve was to remove the need for 'return' within the if statements. I was hoping that this wasn't necissary as it closely resembles c programming. Perhaps this question could be answered in class.
