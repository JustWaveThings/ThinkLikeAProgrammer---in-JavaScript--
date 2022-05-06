#Luhn Checksum Validation Fixed Length - Exercise 

- See the [pdf](/chapter_2/luhnChecksumValidationFixedLength_inProgress.pdf) for the problem explanation and my analysis. Below is my pseudocode and then the plan is to code it out to make a working example.

##Psuedocode -
```
A)  We have to read and process each digit one at a time (left to right). We can’t store the numbers. 

    We would need a variable to store the processed output from each digit that would sum to the previous output - this would allow us to discard the previous inputs.

    We would need to index the numbers to know which is even or odd

    We would need a variable for the current number
```

let cumSum = 0;
let curNum = 0;
let currNumIndex = 1 // make sure to do action then increment so the index matches 1,2,3 and not 0, 1, 2


```
B) Every other number is doubled

    A) We’d need to make a counter variable that is incremented at the end of each id digit.  (taken care of in A) At the beginning of the beginning of the digit processing, we’d need to check to see if it was an even or odd number.  If even, the digit would need to be doubled. If odd, it would just be added on. 

C)If the number doubled is two digits, they are added inline to checksum 
```



let oddEven = (curNumIndex/2);

if oddEven modulo is not zero, then it's an odd number, then we'd just add curNum to cumSum. Else we'd need to double the number.

I'm thinking a nested if statement or switch statement would be the best structure for this part of the exercise.
