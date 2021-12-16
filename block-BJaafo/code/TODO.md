### Write two tests for the following functions

#### Get full name

1. Write a function that takes two input `firstName` and `lastName` and returns full name. You will get the full name by adding first and last name with an space.
2. After writing the function write two tests for above function
3. Make the first test fail and look at the output
4. After making the first test fail do you see the output of the second test?


function fullName(firstName, lastName) {
    return firstName + " " + lastName;
}

let result = fullName("Ashwini", "Gupta");

let expected = fullName

if(result !== expected) {
    throw new Error(`${result} is not equal to ${expected}`)
}



result = fullName("Ashwini", "Gupta");

expected = "Ashwini Gupta";

if(result !== expected) {
    throw new Error(`${result} is not equal to ${expected}`)
}

#### Calculate total amount

1. Write a function that takes two input `amount` and `taxRate` and returns the total amount by `amount + (amount * taxRate) `
2. Write two tests for the above function
3. Make the first test fail and look at the output
4. After making the first test fail do you see the output of the second test?


function totalAmount(amount, taxRate) {
    return amount + (amount * taxRate);
}

let result = totalAmount(1000, 5);

let expected = 5000;

if(result !== expected) {
    throw new Error(`${result} is not equal to ${expected}`)
}


result = totalAmount(1000, 5);

expected = 6000;

if(result !== expected) {
    throw new Error(`${result} is not equal to ${expected}`)
}