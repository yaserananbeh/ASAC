# Class-09

## What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

## What is a pure function and how do we know if something is a pure function?

* It returns the same result if given the same arguments (it is also referred as deterministic)
* It does not cause any observable side effects

## What are the benefits of a pure function?

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

   - Given a parameter A → expect the function to return value B
   - Given a parameter C → expect the function to return value D

## What is immutability?

When data is immutable, its state cannot change after it’s created. 

## What is Referential transparency?

if a function consistently yields the same result for the same input, it is referentially transparent
pure functions + immutable data = referential transparency


## What is a module?
as the component in the react but here with the backend we can make a seperate files (modules ) that contain a js code and require them whenever we need to use their code .

## What does the word ‘require’ do?
the require basicly make the call or import for the module inside another file 
## How do we bring another module into the file the we are working in?
inside it we put module.export and the peice that we need to share with the other files then inside the another file we use the require to import the exported module 

## What do we have to do to make a module available?
module.export (the part that we need to share with the other files)
