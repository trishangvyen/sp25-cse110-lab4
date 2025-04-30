1. At line 12, the index (*i*) that the for block ended off on will be printed into the console. In this situation, it prints 3 which is equal to prices.length. This happens because the index (*i*), is a **var**, which are function-scoped meaning that after the loop ends, *i* still exists and keeps the value it had (3).

2. At line 13, the final value of *discountedPrice* is printed into the console (150). This happens because *discountedPrice* is a **var**, so after the loop, the variable still exists and keeps the last value that was computed in the loop, which is 150.

3. At line 14, the final value of *finalPrice* is printed into the console (150). This happens because *finalPrice* is a **var** and is being updated through each iteration. After the loop, this variable still exists and holds the last value that was computed because **var**s are function-scoped and can still be accessed outside of the for block.

4. This function will return the *discounted* array, being [50, 100, 150]. This is because in the for loop, we are multiplying each original price from to input by 1 minus the discount (0.5). After this, the result is rounded to 2 decimal places to be in currency format and is then pushed into the *discounted* array. After the last iteration of this loop, it's returned.

5. In line 12, we get an error because we are trying to access the variable *i*, but it is unreachable because it is defined within the for block using **let**. The **let** declarator is block-scoped, so *i* only exists within the loop brackets. Once this loop ends, it is no longer accessible. Therefore, we receive a ReferenceError where *i* is not defined.

6. Line 13 returns a ReferenceError because *discountedPrice* is declared within the for block using **let**, which is block-scoped. Therefore, line 13 cannot access the *discountedPrice* variable because it is called outside of the for loop brackets whilst *discountedPrice* is only defined within the loop.

7. Line 14 returns the final value of *finalPrice* (150) because it is declared outside of the for loop using **let**, which is block-scoped, but since line 14 is still within the brackets of its declaration, it can access it without errors. Within the loop, *final Price* is still accessible because the loop is still within the brackets of its original declaration. After the loop is done, *finalPrice* keeps the value of 150 and in result, line 14 prints 150 into the console.

8. The function will return the *discounted* array, [50, 100, 150], because in the for loop, we are multiplying each original price from to input by 1 minus the discount (0.5). After this, the result is rounded to 2 decimal places to be in currency format and is then pushed into the *discounted* array. After the last iteration of this loop, it's returned. There are no errors because *discounted* is declared with **let** within the function brackets and the return line is also within the brackets, so we have no reference errors. We also have no problems with any other variables because although *i* and *discountedprice* are declared with **let** within the for loop, they are only utilized and accessed within that loop. Same goes for *finalPrice*, it is only accessed within its brackets.

9. At line 11, we get an error because we are trying to access the variable *i*, which is unreachable because it is defined within the for block using **let**. The **let** declarator is block-scoped, so *i* only exists within the loop brackets of where it's declared. Once this loop ends, it is no longer accessible. Therefore, we receive a ReferenceError where *i* is not defined since line 11 is outside of the loop brackets.

10. At line 12, the **const** *length* is printed (3) because when it was declared, it stored the length of the prices array input, which contains 3 elements. The declarator **const** allows us to access it within the same block its declared in because it is block-scoped. Because line 12 is still within the function block, it is able to access *length*.

11. This function will return the *discounted* array, [50, 100, 150], because in the for loop, we are multiplying each original price from to input by 1 minus the discount (0.5). After this, the result is pushed into the *discounted* array. After the last iteration of this loop, it's returned. There are no errors because all variables are declared using **const** or **let** and are only accessed within each of their respected blocks that they were declared in. In addition to this, no variables are being reassigned incorrectly.

12. The notation for:
    1.  Accessing the value of the name property in the student object: `student.name;`
    2.  Accessing the value of the Grad Year property in the student object: `student['Grad Year'];`
    3.  Calling the function for the greeting property in the student object: `student.greeting();`
    4.  Accessing the name property of the object in the Favorite Teacher property in student: `student['Favorite Teacher'].name;`
    5.  Access index zero in the array of the courseLoad property of the student object: `student.courseLoad[0];`

13. Arithmetic:
    1.  '3' + 2 Output: true, because the string '2' becomes the number 2 and 2 > 1.
    2.  '3' - 2 Output: '32' because the + sign performs string concatenation and integers map to their exact string representation.
    3.  3 + null Output: 3, because null turns in 0 in numeric conversion, so 3 + 0 would output 3.
    4.  '3' + null Output: '3null' because the + sign performs string concatenation and null is converted to 'null'.
    5.  true + 3 Output: 4, because true converts into 1 in numeric conversion and 1 + 3 = 4.
    6.  false + null Output: 0 because numeric conversion turns false into 0 and null into 0, 0 + 0 = 0.
    7.  '3' + undefined Output: '3undefined' because the + sign performs string concatenation so undefined is converted to 'undefined'
    8.  '3' - undefined Output: NaN, because '3' converts into the integer 3 while undefined cannot be converted into a number in numeric conversion, resulting in NaN.

14. Comparison:
    1. '2' > 1 Output: true, because '2' is converted into the number 2 and is then compared to 1, since 2 is greater than 1, it returns true.
    2. '2' < '12' Output: false, because both operands are strings so JS uses dictionary order to compare them. Since '2' comes after '1' in lexicographical order, it returns false.
    3. 2 == '2' Output: true, because the string, '2', becomes the number 2, and 2 is equal to 2, so it returns true.
    4. 2 === '2' Output: false, because === checks for strict equality, so there is no type conversion. Since 2 is a number and '2' is a string, they are not strictly equal to each other, returning false.
    5. true == 2 Output: false, because true converts into the integer, 1, and 1 is not equal to 2, returning false.
    6. true === Boolean(2) Output: true because Boolean(2) converts into true since any number that is not zero is true, so this turns into true === true, which will return true.

15. The difference between == and === is that == compares 2 values after converting them into a common type while === is strict equality and does not convert types, so both operands must be the same type and value for it to be true.

16. in JS file part2-question16.js

17. The result of the function call will be: [2,4,6]. This is because first, the modifyArray function takes the array, [1,2,3], and the callback, doSomething. Inside modifyArray, an empty array named newArr is create and we loop through each item, using the doSomething function as callback to modifyArray. So, in every iteration of the loop, we are calling doSomething onto array[*i*] and pushing the output of doSomething into newArr. After the loop ends, the function returns newArr, which is [2,4,6].

18. in JS file part2-question18.js

19. The output of the code is: 1, 4, 3, 2 with each number being on a new line. 2 was printed with a delay because it was scheduled with setTimeout to run after 1 second. On the other hand, 1 and 4 printed immediately with no delay and 3 prints after the main code because setTimeout was used, even though it was scheduled to run after 0ms.