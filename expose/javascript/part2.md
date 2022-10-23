1.  The value of i, 3, will be logged to console/printed, because var allows variables to be accessed outside of the block they were defined in (ie i is accessed outside of the for loop). 
2.  150 will be printed, because the last value of discountedPrice will be prices\[2\]*(1-0.5), which is 300\*0.5 or 150. Again, var will allow discountedPrice to be printed outside of its defined scope, or outside of the for loop. 
3.  150 will be printed, as finalPrice will round 150 (the last value of discountedPrice) to the nearest int- or 150, and as finalPrice is defined in the scope of this function (but var would let it be printed even if it was defined within a block in this function).
4.  This function returns \[ 50, 100, 150 \], as discounted pushes finalPrice, or 0.5 times each of the values in price rounded to the nearest integer. Thus, \[100, 200, 300 \] would be halved to create the array \[ 50, 100, 150 \]. Also, discounted is defined in the scope of this function with var. 
5.  Error, i is not defined outside of the for loop's scope due to the usage of let while declaring it, thus it cannot be logged on line 12. 
6.  Error, discountedPrice is not defined outside of the for loop's scope due to the usage of let while declaring it, thus it cannot be logged on line 13. 
7.  150 will be printed, as finalPrice will round 150 (the last value of discountedPrice) to the nearest int- or 150, and as finalPrice is defined w/ let in this scope of this function on line 4. 
8.  This function returns \[ 50, 100, 150 \], as discounted pushes finalPrice, or 0.5 times each of the values in price rounded to the nearest integer. Thus, \[100, 200, 300 \] would be halved to create the array \[ 50, 100, 150 \]. Also, discounted is defined in the scope of this function with let. 
9.  Error, i is not defined outside of the for loop's scope due to the usage of let while declaring it, thus it cannot be logged on line 11.  
10. 3 will be printed, as the constant variable length is assigned to the length of price (3), then it isn't reassigned, so there isn't an error. 
11. \[50, 100, 150 \], as the constant variable discountedPrice is assigned to 0.5 \* the values of price, and this would be an error as discountedPrice is reassigned at every iteration of the for loop, but since the variable discountedPrice is redefined at each iteration, there is no error and an updated value of discountedPrice is pushed to discounted, which is returned. Thus, prices => \[100, 200, 300 \] would be halved to create the array \[ 50, 100, 150 \], which is returned. 
12. <br>
    A. console.log(student.name);<br>
    B. console.log(student["Grad Year"]); <br>
    C. student.greeting();<br>
    D. console.log(student["Favorite Teacher"]["name"]);<br>
    E. console.log(student.courseLoad[0])<br>
13. <br>
    A. '32' : integer 2 maps to string '2'<br>
    B. 1 : string '3' maps to integer 3<br>
    C. 3 : null type maps to integer 0 <br>
    D. '3null': null type maps to 'null' string, concatenation <br>
    E. 4 : boolean true maps to integer 1 <br> 
    F. 0: boolean false maps to integer 0, null maps to integer 0 <br>
    G. '3undefined' : undefined type maps to string 'undefined', concatenation <br>
    H. NaN : results in not a number, '3' string can map to 3 integer, but undefined doesn't map to an integer <br>
14. <br>
    A. true: '2' string maps to 2 integer <br>
    B. false: strings are compared letter by letter, so '2' < '1' is deemed true as '2' maps to integer 2 and '1' to int 1 <br>
    C. true: '2' maps to integer 2 which = 2 <br>
    D. false: === checks the equality without type conversion, since integer 2 isn't equal to '2', this is false <br>
    E. false: boolean true maps to integer 1, which is not equal to 2. <br>
    F. true: 2 is converted to to the true boolean as only "empty" values map to false, and the boolean trues are equal <br>
15. == checks for equality with type conversion, however === checks for strict equality, without type conversion- so even if values might be mapped to equal values, if they aren't the same type, they won't be considered equal. 
16. answer in part2-question16.js 
17. [ 2, 4, 6 ]: we pass in the array [ 1,2,3 ] into the modifyArray() function, which creates a new array and takes the values from the array passed in and passes them into the doSomething() function, which multiplies these values by 2, then these doubled vallues are returned and pushed into newArr, which is returned. Thus, the modifyArray() fn returns the values of the [ 1,2,3 ] array doubled.
18. 1 <br> 4<br> 3<br> 2<br>