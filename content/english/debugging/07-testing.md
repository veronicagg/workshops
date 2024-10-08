---
title: "Step 3 - Testing"
difficulty: "Intermediate"
weight: 8
draft: false
---

You’ve implemented the fix(es) for your bug(s). Naturally, the first thing you do is recompile your code and run it. If it looks right, you’ve fixed the bug! For smaller projects, this works relatively well. Larger projects might be more difficult since it takes much longer to compile. Typically, these have automated tests that are run automatically after updates are made to the codebase so programmers don't even need to worry too much about this step (except for the programmers making the tests!).

In testing you already know or have a good idea of where the bug will occur, and so in your tests you’ll want to intentionally run that code to make sure that code is correct. Testing is so important that a whole software development methodology revolves around it (test-based development)!

Sometimes fixing a bug may introduce another bug, which is called a _regression_. It's very normal to sometimes have multiple iterations of bug fixes!

## Unit Tests
Always start small with your tests. This idea is taken from scientific experiments: if you reduce the number of factors (independent variables) that are in play, you can narrow down the cause more easily. These are called unit tests. Rather than testing if the entire program or part works, a unit test looks at a specific part. A unit test could call one function that does not call other functions to see if it outputs the correct/expected value.

For example, let's say you have a calculator app that can add, subtract, multiply, and divide numbers. You could write a unit test to test just the addition function by giving it 2 numbers and checking to see if it returns the right value.  

## Integration Tests
Only once your unit tests have succeeded should you start integration tests. Integration tests look at how multiple components of your program work together to see if they output the correct/expected value. An integration test could call a function that calls many other functions, or affects many different parts of the program.

Just because your unit tests work doesn’t mean your integration tests work. You could write an integration test for your calculator app by testing a series of arithmetic operations, such as performing addition and then multiplication, and checking the result.
