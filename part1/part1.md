## 1a
- 1. Line 9 prints "values added:  20"
- 2. Line 13 prints "final result:  20"
- 3. Line 9 prints "values added:  20"
- 4. Line 13 errors because "let" only defines a variable within the "if" block. Outside of the "if" block, 'result' is not defined when we try to print it on line 13.
- 5. Line 9 isn't reached because we try to assign to 'result' on line 7. 'result' is a const, so the program errors. 
- 6. Line 13 isn't reached because we try to assign to 'result' on line 7. 'result' is a const, so the program errors. 

## 1b
- 1. Line 12 prints '3' because the value of 'i' will be equal to prices.length after the for loop. The length of prices is 3, so 'i' will also be 3 and '3' is printed out.
- 2. Line 13 prints '150' because the last value if 'discountedPrice' is equal to the last value of 'prices' multiplied by (1-discount). This is equal to 300*(1-0.5) = 150.
- 3. Line 14 prints '150' because the last value of finalPrice equals the lastt value of discountedPrice calculated. This would be Math.round(150*100)/100, which is equal to 150.
- 4. The function returns [50,100,150]. This is because with a discount of 0.5, each price that is initially passed into the function is multiplied by (1-0.5) = 0.5, essentially halving each price. 
- 5. Line 12 is an error because 'i' is of the 'let' type. This means that it only has block scope within the for loop, and therefore does not exist within the scope that 'console.log' is within.
- 6. Line 13 is an error because 'discountedPrice' is of the 'let' type. This means that it only has block scope within the for loop, and does not exist within the scope that 'console.log' is within.
- 7. Line 14 would print out '150' because it would depend on the last price of 'discountedPrice', which depends on the last price of 'prices'. After calculations, 'disconutedPrice' is equal to 150, and after calculating Math.round(150*100)/100 the result is 150, the vlaue of 'finalPrice'.
- 8. This function would return [50,100,150] because with a discount of 0.5, each price passed in is essentially halved. Therefore [100,200,300] becomes [50,100,150].
- 9. Line 11 errors because 'i' is of the 'let' type, meaning that it only has block scope within the for loop. When we try to print it out with 'console.log', 'i' does not exist within that scope, therefore erroring.
- 10. Line 12 prints out '3' because 'length' was defined within the function scope, never modified, and set equal to the length of 'prices'. 'prices' was 3 elements long, so the length was '3'.
- 11. The function returns [50,100,150] because each price is subtracted with the discount, which is 0.5. This means that [100,200,300] becomes [50,100,150].

12. 
a. student.name
b. student['Grad Year']
c. student.greeting()
d. student['Favorite Teacher'].name
e. student.courseLoad[0]

13.
a. 32 - the 2 casts to a string, and string concatenation happens
b. 1 - the 3 casts to an int, and 3-2 = 1
c. 3 - the null becomes 0, and 3+0 = 0
d. 3null - null casts to a string, and string concatenation happens
e. 4 - true casts to 1, and 1+3 = 4
f. 0 - false casts to 0 and null is also 0, so 0+0=0
g. 3undefined - undefined casts to a string, and then string concatenation happens
h. NaN - undefined becomes NaN when casted for subtraction, and anything subtracted with NaN is NaN

14.
a. true - 2 is casted to int, and 2>1 is true
b. false - 2 and 12 are casted to int, and 2<12 is true
c. true - 2 is casted to int and 2 is equal to 2
d. false - the types are different, so false
e. false - true is casted to 1, and 1 does not equal 2
f. true - truthy value of 2 is true, and true equals 2

15.
== checks for equality while typecasting different variable types on each side of the operator. However, === checks for equality without typecasting. 

17.
The result should be [2,4,6] becuase we pass in the array [1,2,3] and the function calls callback on each value of the array, adds it to an output, and returns the output. Therefore each value is multiplied by 2 and returned in an array.

19. 
The output is:
1
4
3
2
