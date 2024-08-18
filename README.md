# Left Recursion Removal in Context-Free Grammar

This C++ program is designed to process context-free grammars and remove left recursion. It reads a set of production rules, identifies any left recursion, and then outputs the transformed grammar.

## Overview

The code performs the following tasks:
1. **Input Handling**: Accepts a number of production rules and reads them from the user.
2. **Processing**: Identifies and removes left recursion from the grammar.
3. **Output**: Prints the transformed grammar or the original grammar if no left recursion was detected.

## How It Works

### Functions

#### `vector<string> split(const string& str, char delimiter)`

Splits a given string `str` into a vector of substrings using the specified `delimiter`. It also trims leading and trailing whitespace from each substring.

**Parameters:**
- `const string& str`: The string to be split.
- `char delimiter`: The character used to split the string.

**Returns:**
- `vector<string>`: A vector containing the split substrings.

### Main Program

1. **User Input**: The program prompts the user to enter the number of productions and the production rules in the format `A -> Aa | b`.
2. **Processing Productions**:
   - Extracts non-terminal symbols and production rules.
   - Identifies rules with left recursion.
   - Transforms the grammar to remove left recursion.
3. **Output**: Displays the transformed grammar or the original grammar if no left recursion was present.

## Compilation and Execution

1. **Compile**: Use a C++ compiler like `g++` to compile the code.
   g++ -o grammar_processor grammar_processor.cpp
