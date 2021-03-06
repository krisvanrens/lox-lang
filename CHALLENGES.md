# Challenges

Answers for challenges for the book "Crafting Interpreteters".

## Chapter 1

1. Markdown, CSS, SCSS, SASS, HTML, Mustache.
2. Done.
3. That's my day job; so: done.

## Chapter 2

1. I wrote a mini-language for scatter-gather building before using Flex and Bison.
2. It's very complex. The burden of having to ship a full compiler (for which architecture?) for a runtime, and the compilation overhead (memory/compute resources) itself during running.
3. Ease of implementation of the REPL, and for facilitating the user.

## Chapter 3

1. There's no multiple inheritance. This will probably very much complicate the language and introduce difficulties such as the dreaded diamond. Also, there are no constant values.
2. What are the default semantics for copying/moving? The answer is copying in the implementation, but it could be move semantics for a more efficient implementation. But this would inherently mean introducing C/C++-style references or pointers into the language.
3. Generics would be great, but this will hugely increase the complexity quite likely. Less costly would be the adding of convenience operators such as prefix/postfix in-/decrement like C and C++ have. The same holds for the compound assignment/arithmetic operators such as `+=`/`-=`/`*=`/`/=`. For system-programming domains bit operations and word-sized types would be beneficial.

## Chapter 4

1. The lexical grammars for Haskell and Python are not regular, because they use indentation space as an active part of it.
2. In Coffeescript, parentheses for function calls are optional. This means the lexical grammar rules must be such that the space is mandatory, even when using parentheses. In C function macros, the preprocessor expects _no_ space between the macro name and the parentheses of the parameter list. In Ruby the same holds as for CoffeeScript.
3. Multiline strings, or perhaps multiline comments.
4. Done (including nesting). Nesting is slightly more difficult because it requires recursion.

## Chapter 5

1. `// TODO`
2. `// TODO`
3. `// TODO`

## Chapter 6

1. The comma operator simply is a binary operator with the lowest precedence. Implemented.
2. The ternary operator has low precedence, right above the comma operator. The ternary operator is right-to-left associative. The middle expression (between the `?` and the `:`) is parsed as if parenthesized; its precedence with respect to `?:` is ignored. Implemented.
3. The error productions must be put at the end (of the `primary` production). Implemented.

## Chapter 7

1. I would tend to prevent comparing objects of different types, because most often this is a bug (IMHO). A static type system is another story altogether, but I would definitely steer towards a language that supports the programmer into fixing bugs early on, instead of them having to deal with a "free for all" language like JavaScript. In order to support comparing various types I would add type conversion utilities for the programmer to explicitly mark the comparisons.
2. Done.
3. Done.

## Chapter 8

1. No, won't do.
2. Done.
3. It prints '3'.

## Chapter 9

1. `// TODO`
2. `// TODO`
3. `// TODO`

## Chapter 10

1. `// TODO`
2. `// TODO`
3. `// TODO`

## Chapter 11

1. `// TODO`
2. `// TODO`
3. `// TODO`

## Chapter 12

1. `// TODO`
2. `// TODO`
3. `// TODO`

## Chapter 13

1. `// TODO`
2. `// TODO`
3. `// TODO`
