1. The value of i (price.length) will be printed out because unlike the let keyword, the var keyword has no conception of code blocks scope so anything in a code block is visible to the rest of the function. Thus no error. 
2. The value of the last discounted price will be printed becasue once again the var keyword can be visible thorughout the function so no error.
3. This will print the final rounded discounted price of the last price in the price list because the variable was decalred with the var keyword so it has visibility within the function.
4. it will return the list: [50,100,150] since we go through each item in prices and multiply the original prices with the discount and insert each of the new prices into the new list thus we get the returned list. 
5. An error will occur because in a for loop, the for loop (inlcuding i) and whats in the for loop are considered to be in the same code block. Thus the console.log statement and foor loop are in different code blocks so we get an error since we try to access something from a different code block. Code blocks do apply for the let keyword.  
6. An error will occur once again for the same reason stated in question 1.
7. This will print the final rounded discounted price of the last price in the price list because the variable was decalred with the let keyword outside of the for loop so this will not cause an error since the console statement is in the same code block as the declaration.
8. it will return the list: [50,100,150] since we go through each item in prices and multiply the original prices with the discount and insert each of the new prices into the new list thus we get the returned list (If we ignore the errors that is).
9. An error will occur because in a for loop, the for loop (inlcuding i) and whats in the for loop are considered to be in the same code block. Thus the console.log statement and for loop are in different code blocks so we get an error since we try to access something from a different code block because the let declaration uses code blocks. 
10. Since let and const have the same notion of code block scope, this line will produce an error since the discountedPrice is defined in a different block than the console and the console is trying to get the discounted value. Note the error is not because of it trying to change a const value since each time we iterate the for loop the const value gets created each time. 
11. This would give us a error saying that we cannot change a const vairable's reference after initlaizing it but if we ignored the error but still treated it like a const then it will print 0 since we cannot change the variable after its been declared and notice we have access to it since it is in the same code block as the log. 
12. Techincally this function wouldnt return anything since there are several errors with regrards to scope and changing const values. But if we ignore the errors, it will return the list: [0,0,0] since we go cannot change finalprice's refernece like in line 7 so finalPrice will remain 0 based on the way we try reassigning final price. Additionally we push final price (0) to the array 3 times. Notice that it will not output [] even with the const in discounted because const just means we cannot change its reference. And we arent, we are only chanigng the contents being held at the reference. Thus we get [0,0,0], assuming we ignore errors.
13. - a) student.name
    - b) student['Grad Year'] 
    - c) student.greeting()
    - d) (student['Favorite Teacher']).name
    - e) (student.courseLoad)[0]
14. - a) '32'
    - b) 1
    - c) 3
    - d) '3null'
    - e) 4
    - f) 0 
    - g) "3undefined"
    - h) NaN
15. - a) true
    - b) false
    - c) true
    - d) false
    - e) false
    - f) true
16. == Will convert the objects so they are of the same type(int) then will compare the two after conversion. Whereas === will compare the two objects without conversions.
17. The first if branch 2 == true will evalute to false because it will convert the two types to numbers so 2 is already an int so it does nothing, but it will convert true to an int which will be 1. Then when we compare 2 does not equal 1 thus we get false. But when we convert 2 to a boolean, since any non zero number when coverted to a boolean returns true the second branch is enter and prints 'How are you?'
18. see part1-question18.js
19. The result will be [6,8,10] so at the first iteration we push the result of doSomething given 1 and a function that doubles the input. Then doSomething will return double(1+2) then double(3) returns 6 and we push this to the array. So at each step we add 2 to the current number, double it then push it to the array. Note that we dont get a const error since we are not changing the reference of the const variable on the contents of the variable.
20. see part1-question20.js
21. The output of the code is console statements in the order: 1 4 3 2.
    