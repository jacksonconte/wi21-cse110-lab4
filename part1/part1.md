# Part 1 answers
1. Line 11 will print the length of prices - 1 (i) because var cannot be block-scoped to the for loop and will instead be function-scoped to discountPrices().
2. Line 12 will print the final (unrounded) discountedPrice that is calculated because var cannot be block-scoped to the for loop and will instead be function-scoped.
3. Line 13 will print the final (rounded) finalPrice in the function output because var will be function-scoped.
4. The function will return [50, 100, 150] because each number in [100, 200, 300] will be multiplied by (1 - 0.5 = 0.5). This is an exact number so rounding is negligible. Each halved price will be pushed to discounted after rounding, and as such the array [50, 100, 150] will be returned.
5. Line 11 will result in an error, since let will be scoped to the code block in the for loop.
6. Line 12 will result in an error, since let will be scoped to the code block in the for loop.
7. Line 13 will print the last price in discounted, since let is scoped to the code block of the function discountPrices.
8. The function will return [50, 100, 150] because the function works the same way as the function for questions 1-4 and there are no variable errors outside of lines 11 and 12 (finalPrice and discounted are modified but not re-declared with let).
9. Line 11 will result in an error, since let will be scoped to the code block in the for loop and is not defined outside of it.
10. Line 12 will result in an error, since const will be scoped to the code block in the for loop and is not defined outside of it.
11. Line 13 will print 0, because any attempt to modify finalPrice in the for loop will result in an error, as it is a const. Therefore, it will always be guaranteed to print the original value of finalPrice.
12. Because finalPrice is defined to always be 0 and cannot be modified in the same scope (the function), any time finalPrice is pushed to discounted, it will simply add a 0 to the array. Therefore, the function will return [0, 0, 0].
13. Notation

    a. student.name
    
    b. student['Grad Year']
    
    c. student.greeting()
    
    d. student['Favorite Teacher'].name
    
    e. student.courseLoad[0]
    
14. Arithmetic

    a. 5; '3' is automatically converted to number with + operator
    
    b. 1; '3' is automatically converted to number with - operator
    
    c. 3; null is auto-converted to 0
    
    d. '3null'; lhs is string so null is converted to a string and concatenated
    
    e. 4; true is converted to 1 with + operator
    
    f. 0; false and null are both converted to 0
    
    g. "3undefined"; lhs is string so undefined is converted to string
    
    h. NaN; - operator is not overloaded for string operation, so 3 is converted to a number and undefined is converted to NaN.
    
15. Comparison

    a. true; different types so '2' is converted to number
    
    b. false; '2' is greater in lexicographical order than '1'. Comparison stops here.
    
    c. true; different types so '2' is converted to number
    
    d. false; strict equality differentiates types
    
    e. false; true is converted to the number 1, and 1 != 2
    
    f. true; nonzero value 2 is converted to true with boolean function; strict equality passes since types are same
    
 16. The == operator automatically converts both operands to numbers, while the === operator checks types first and returns false if they are different. It only returns true if types *and* values are equal.
 
 17. 'How are you?' is printed because the == operator converts true to a number (and 2 != 1). However, the implicit Boolean conversion done by the else if statement on 2 returns true for any nonzero value. Therefore, the else if branch is chosen and 'How are you?' is printed.
 
 18. in JS file
 
 19. For each element in the array [1, 2, 3], there is a new element added to newArr that is the result of doSomething with that as its input and a doubling function. doSomething takes its input function and calls it with the parameter of its input number + 2. Therefore, the first iteration pushes (1 + 2) * 2 = 6, the second iteration pushes (2 + 2) * 2 = 8, and the third iteration pushes (3 + 2) * 2 = 10. Therefore, newArr is returned, or [6, 8, 10].
 
 20. in JS file
 
 21.
    1
    3
    4
    2
