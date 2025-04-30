1. On line 12, the code will print out ``3`` because var was used to declare i. This means that i has a function scope, allowing it to be accessed outside the for loop, and by the rest of the function
2. On Line 13, the code will print out ``150`` because discountedPrice was declared with var, allowing discountedPrice to be accessed through the entire function
3. Line 14 would also print out ``150`` because finalPrice was declared with var, giving it a function scope, and it was last updated to 150.
4. The function returns ``[50, 100, 150]`` because it applies a 50% discount to each price, rounds the result, and returns the array of final prices.
5. Line 12 will throw a reference error because i was declare with let, which is a block scope, and it therefore can't be accessed outside the loop
6. Line 13 tries to access discountedPrice, which was declared with let inside the for loop. Since let is block-scoped, it is not accessible outside the loop block and will throw a reference error
7. Line 14 will print out `150` because finalPrice is declared with let at the function level and updated inside the loop. Its last value is 150, and it is still in scope at line 14.
8. This function returns `[50,100,150]` because the function applies a 50% discount to each price and saves it in discounted which is then returned at the end of the function. Discounted is declared with let, but in the highest level of the function, same level as the return statment, so it is accessible.
9. Line 11 will cause a reference error because i was declared with let inside the for loop, which means that it is only accessible in the for loop. This means that it cannot be accessed on line 11.
10. Line 12 will print out `3` because length is declared with a const outside the loop, which means that it is accessible by console.log(length)
11. This function will return `[50,100,150]` because const allows the contents of the array to be changed, but not the binding. However, push are still allowed for arrays declared with const.
12. Answers for Q12 (using numbers instead of letters)
    1.  student.name
    2.  student["Grad Year"]
    3.  student.greeting()
    4.  student["Favorite Teacher"].name
    5.  student.courseload[0]
13. Arthmetic Questions
    1. The result is 32, because the 2 is converted from number form to string form, and the strings are concatenated
    2. The result is 1, because - is an arthmetic operator, so the 3 is coerced to a number
    3. The result is 3, because in the context of 3 + null,  null is equivalen to 0 and 3 + 0 = 3
    4. The result is 3null, because in '3' + null, null becomes a string "null" and the two strings are then concatenated
    5. The result is 4, because in the context of 3 + true, true is equal to 1. 3 + 1 = 4
    6. The result is 0, because in this context both null and false are equivalent to 0. And 0 + 0 = 0
    7. The result is 3undefined, as undefined is changed to a string 'undefined' and the two strings are concatenated
    8. The result is NaN, because - is an arthmetic operator and undefined is NaN in this context. So it is 3 - NaN is NaN
14. Comparison Questions
    1.  The result is true. In a comparison context, '2' is coerced to a number form and compared to 1, and 2 > 1 is true
    2.  The result is false. Due to context, both are changed to numbers and 2 > 12 is false 
    3.  The result is True. == does a type coersion and compares.
    4.  The result is False. === compares not only the value, but also the type. And since one is a string and the other is a number, it is false
    5.  The result is False. True is equivalent to 1, and 1 != 2 which means the result is false.
    6.  The result is True. Boolean(2) is equal to true, and so true === true results in true (both same type and value)
15. == checks if the variables are equal after a type coersion. However, === checks if the types and values of the variables are the same.
16. answer is on part2-question16.js
17. The final result will be `[2,4,6]`. The steps were
    1.  The `modifyArray` function loops through each number in the array `[1, 2, 3]`.
    2.  For each number in the array, the callback function doSomething is called and it doubles the number.
    3.  After doubling the number, it is pushed to newArr
    4.  doSomething(1) results in 2, and then pushes 2 to newArr
    5.  doSomething(2) results in 4, then pushes 4 to newArr
    6.  doSomething(3) results in 6, then pushes 6 to newArr
18. Answer on part2-question18.js
19. The output would be
    1
    4
    3
    2
    because console.log(1) is the first line, so it would be the first thing to be outputted. The next two lines have a timeout, so that means console.log(4) on line 5 would be the next thing to output. So 4 would be output. Then line 4 would output 3 before line 3 can output 2. This is because line 4 has a timeout of 0 and line 3 has a timeout of 1000.