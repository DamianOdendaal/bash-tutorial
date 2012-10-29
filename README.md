# About

This project is used for workshop purposes and contains examples of (hopefully) good practices for bash scripting.

# Examples

## Debugging

**Source:** scripts/debugging\_easy\_example.sh and scripts/debugging\_tougher\_example.sh                                      

**The point:** Debugging is hard in bash.

**Assignment:** Find the bugs.

## Syntax

**Source:** scripts/syntax.sh

**The point:** You can do similar things in different ways in bash.

**Assignment:** Try out the different ifs and explain the differences, when to use, and what you prefer.

## Organizing files

**Source:** The project tree.

**The point:** Understand convention over configuration and why it is important to put different types of files in different places.

**Assignment:** How would you organize your files when you have specific scripts for different projects residing in different folders.

## Functions and configuration

**Source:** include/common\_functions.sh include/common\_config.sh

**The point:** Reduce complexity, enhance testability, and reusability.

**Assignment:** Go through the functions and try to understand them. Write your own function.

## Return values and return statuses

**Source:** include/common\_functions.sh (functions: \_is\_snapshot, \_start, \_find\_version\_from\_pom and \_delete)

**The point:** Understand the differences betwwen a return value and a return status.

**Assignment:** Revisit the functions and explain what the different functions return (values and/or statuses)

## Pitfall return values

**Source:** scripts/pitfall\_return\_values.sh

**The point:** Understand a common pitfall when using return values.

**Assignment:** Comment in the echo statement in the function and see what happens. Why?

## Pitfall return statuses
**Source:** scripts/pitfall\_return\_status.sh

**The point:** Understand a common pitfall when using return statuses.

**Assignment:** Why do the two statements return different statuses?

## Including common functionality

**Source:** include/includes.sh

**The point:** Understand reusability by sourcing other files.

**Assignment:** Write a function in a file and include and use it in a script.

## Debugging revisited

**Source:** include/common\_functions.sh

**The point:** Understand how you can debug your scripts without executing "dangerous" commands. Understand the -x and the set +e set -e constructs.

**Assignment:** Write debugging for a function or script where it is lacking.

## Logging

**Source:** scripts/logging.sh scripts/rotating\_log.sh  and include/log.sh

**The point:** Understand how you can write your own logging framework.

**Assignment:** Write logging configuration to switch betwwen logging to file and stdout.

## Unit testing framework

**Source:** tests/runAll.sh

**The point:** Example of how you can syntax check and run all your tests.

**Assignment:** MAke running of tests part of your build (scripts/package.sh)

## Unit testing using the && and || operators

**Source:** tests/testMs.sh

**The point:** An example of how you can unit test bash functions using the && and || operators.

**Assignment:** Write a unit test. Is this readable?

## Unit testing with asserts

**Source:** bashUnit/asserts.sh and tests/testVersionCheck.sh

**The point:** An example of how you can unit test bash functions using asserts.

**Assignment:** How does assertEquals differ from the assertTrue in e. g. jUnit? Write an assertTrue function and a test that uses it. Is this more readable?

** Bonus assignment:** Write an assertArrayEquals function and a test that uses it.

## Simple deploy and rollback

**Source:** scripts/deploy.sh and scripts/rollback.sh

**The point:** These scripts are not very testable.

**Assignment:** Make the scripts testable.

