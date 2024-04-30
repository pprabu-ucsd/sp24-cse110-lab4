1. Line 12 will print out ```3```, as it prints out the value of variable ```i```, which is the representation of how many times the loop ran, and since the length of the array ```prices``` is 3, then Line 12 will print out ```3```. Since all variables are defined with ```var```, there is no issue with scope for the use of variables.
2. Line 13 will print out ```150```, as it prints out the value of variable ```discountedPrice```, which is the final calculated discounted price after the loop runs. Since the final value of the array is ```300```, and the discount is ```0.5```, then Line 13 will print out the value of 300 times 0.5, which is ```150```. Since all variables are defined with ```var```, there is no issue with scope for the use of variables.
3. Line 14 will print out ```150```, as it prints out the value of variable ```finalPrice```, which is the final calculated discounted price after the loop runs after rounding. Since the final value of the array is ```300```, and the discount is ```0.5```, then Line 13 will print out the value of 300 times 0.5 rounded, which is ```150```. Since all variables are defined with ```var```, there is no issue with scope for the use of variables.
4. This function will return the list of the discounted prices from the original prices given in ```prices```, as the array ```discounted``` stored the final discounted price for each element in the loop. Therefore, the function will return an array of size 3 with discounted prices in the form ```[50, 100, 150]```. Since all variables are defined with ```var```, there is no issue with scope for the use of variables.
5. Line 12 will return an error, as variable ```i``` is defined with ```let```, so it is only applicable in a block scope, not a function-wide scope. Since Line 12 is outside of the block scope of ```i```, then ```i``` is not defined for Line 12, and will return an error.
6. Line 13 will return an error, as variable ```discountedPrice``` is defined with ```let```, so it is only applicable in a block scope, not a function-wide scope. Since Line 13 is outside of the block scope of ```discountedPrice```, then ```discountedPrice``` is not defined for Line 13, and will return an error.
7. Line 14 will print out ```150```, as it prints out the value of variable ```finalPrice```, which is the final calculated discounted price after the loop runs after rounding, which is 300 times 0.5 rounded, equaling ```150```. Additionally, since Line 14 is in the block scope for variable ```finalPrice```, it will not return an error.
8. This function will return the list of the discounted prices from the original prices given in ```prices```, as the array ```discounted``` stored the final discounted price for each element in the loop. Therefore, the function will return an array of size 3 with discounted prices in the form ```[50, 100, 150]```. Additionally, since the use of array ```discounted``` when returned is in the block scope of the variable's definition, there will be no error.
9. Line 11 will not print anything, as variable ```i``` is only defined in the scope of the for loop, so when Line 11 looks to print the value of ```i``` to the console, it does not exist, resulting in an error.
10. Line 12 will print ```3```, as variable ```length``` represent the length of the array ```discounted```, and since Line 12 is within the scope of variable ```length```'s declaration and initialization, it will not result in an error, and return the length of the array ```discounted```, which is 3.
11. This function will return the list of the discounted prices from the original prices given in ```prices```, as the array ```discounted``` stored the final discounted price for each element in the loop. Therefore, the function will return an array of size 3 with discounted prices in the form ```[50, 100, 150]```. Additionally, even though every variable, except for ```i```, is declared using ```const```, since the variables are never reassigned values, there are no errors encountered.
12.  
     * ```student.name```
     * ```student['Grad Year']```
     * ```student.greeting()```
     * ```student['Favorite Teacher'].name```
     * ```student.courseLoad[0]```
13.  
     * ```'3' + 2 = '32'```, since when using addition with the first value being a string, JavaScript assumes that the result should be string concatenation, resulting in ```32```.
     * ```'3' - 2 = 1```, as when using the subtraction sign, JavaScript converts the string value into an integer value, then completes 3 - 2, returning ```1```.
     * ```3 + null = 3```, since when doing arithmetic with integers, null is considered to be 0, so ```3 + null``` is the same as ```3 + 0```, which is ```3```.
     * ```'3' + null = '3null'```, since when using addition with the first value being a string, JavaScript assumes that the result should be string concatenation, resulting in ```3null```.
     * ```true + 3 = 4```, since true in addition of integers is considered as 1, so ```true + 3``` is ```1 + 3```, which results in ```4```.
     * ```false + null = 0```, as in arithmetic, both ```false``` and ```null``` are considered to be 0, so ```false + null``` is the same as ```0 + 0```, which results in ```0```.
     * ```'3' + undefined = '3undefined'```, since when using addition with the first value being a string, JavaScript assumes that the result should be string concatenation, resulting in ```3undefined```. 
     * ```'3' - undefined = NaN```, as when using the subtraction sign, JavaScript converts the string value into an integer value, then completes 3 - undefined, returning ```NaN```, since that expression is not computable.
14.  
     * ```'2' > 1 -> true```, as when comparing strings to numbers, JavaScript converts the string to integers if possible, and since 2 is greater than 1, the returning value will be ```true```.
     * ```'2' < '12' -> false```, as string comparison is done in lexographical order, or from left to right, and since 2 is greater than 1, despite 12 being greater than 2, since the first digit is greater for 2 compared to 12, then the result is ```false```.
     * ```2 == '2' -> true```, as ```==``` is a loose equality comparison, converting the operands before testing for equality, and since ```'2'``` can be converted to an integer, and ```2 == 2```, then it will return ```true```.
     * ```2 === '2' -> false```, as ```===``` is a strict equality comparison, not converting operands before testing for equality, and since the first operand is an integer while the second is a string, it will return ```false```. 
     * ```true == 2 -> false```, since ```true = 1``` in conversion to an integer, and since 1 does not equal 2, it will return ```false```.
     * ```true === Boolean(2) -> true```, since ```Boolean(2) = true```, and so the expression will be ```true === true```, which will return ```true```.
15. The ```==``` operator is an equality operator that compares two values after converting them to a common type, known as a loose equality comparison, while in contrast, the ```===``` operator is an equality operator that compares two values without any type conversion, also known as strict equality comparison.
16. In the file ```part2-question16.js```.
17. The result of ```modifyArray([1,2,3], doSomething)``` is the array value ```[2,4,6]```. The function returns this array value, as all the function does is iterate through the array given in the parameters, then running each individual element of the array through the callback function ```doSomething(num)```, which doubles the value of the element, before pushing it to the array ```newArr```, finally returning ```newArr```.
18. In the file ```part2-question18.js```.
19. ```
    1
    4
    3
    2
    ```