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