# Title


## Quick Refs and Sources 

## Index of Contents

1. [Strings](#1)	
2. [Arrays](#2)

## Strings{#1}

| Description                                      | Syntax                              |
| ------------------------------------------------ | ----------------------------------- |
| Get the length of a string                       | `${#VARNAME}`                       |
| Get a single character                           | `${VARNAME[index]}`                 |
| Get the string from a specific index             | `${VARNAME[index,-1]}`              |
| Get a substring                                  | `${VARNAME[from,to]}`               |
| Replace the first occurrence in a string         | `${VARNAME/toreplace/replacement}`  |
| Replace all occurrences in a string              | `${VARNAME//toreplace/replacement}` |
| Cut a string after a model                       | `${VARNAME%%model*}`                |
| Check if a string starts by a specific substring | `if [[ $VARNAME = "startstr"* ]]`   |
| Check if a string contains a substring           | `if [[ $VARNAME = *"substring"* ]]` |
| Check if a string ends by a specific substring   | `if [[ $VARNAME = *"substring" ]]`  |

## Arrays{#2}

| Description                                         | Syntax                           |
| --------------------------------------------------- | -------------------------------- |
| Create an array                                     | `VARNAME=()`                     |
| Create an array with initial values                 | `VARNAME=(value1 value2 value3)` |
| Push to an array                                    | `VARNAME+=(value)`               |
| Access an array's element                           | `VARNAME[index]`                 |
| Remove first element from an array (shift)          | `shift VARNAME`                  |
| Remove last element from an array (pop)             | `shift -p VARNAME`               |
| Get an array's length                               | `${#VARNAME}`                    |
| Iterate over an array's values                      | `for value in $VARNAME;`         |
| Get index of a value in an array (`0` if not found) | `${VARNAME[(Ie)value]}`          |
| Get index of a value in an array (`${#VARNAME} + 1` if not found) | `${VARNAME[(ie)value]}`          |
| Get an array slice _after_ the specified index      | `${VARNAME:index}`               |
| Get an array slice _after_ the specified index      | `${VARNAME:index:length}`        |
| Check if a value is contained in an array           | `if (( $VARNAME[(Ie)value] ));`  |
| Check if an array is empty                          | `if [[ -z $VARNAME ]]`           |
| Check if an array is not empty                      | `if [[ ! -z $VARNAME ]]`         |
| Remove an element from an array                     | `VARNAME[index]=()`              |

