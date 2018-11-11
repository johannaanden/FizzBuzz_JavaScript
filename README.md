# Question from the course material

## Question 1. 
In your README to the best of your knowledge please explain what the following lines of code do

```
let  fizzBuzz = fs.readFileSync('./src/js/fizz-buzz.js');
eval( fizzBuzz + `\nexports.FizzBuzz = FizzBuzz;`)
```

## Answer
#### Line 1
Creates the vareiable fizzBuzz that is assigned the value of a JavaScript file called fizz-buzz.js

#### Line 2
I really don't know what this line do. I only know that `eval()` is a function that evaluates JavaScript code that is represented as a string.

________________
## Question 2. 
In your README to the best of your knowledge please explain why we are placing the

```
let fizzBuzz = new FizzBuzz
```

outside the it block?

## Answer
So it's can be used by more than on it block.

________________
## Question 3. 
In your README to the best of your knowledge please explain the difference between using `===` and `==` in JS?

## Answer
Both `==` and `===` checks if something is equal to something else. The difference is that `===` also check the type of the element.

________________
## Question 4. 
In your README to the best of your knowledge please explain why we are moving `(number % 5 === 0)'` to the top?

## Answer
If the first condition in the if statement is True, then the remaining terms will not be evaluated.
________________
## Question 5. 
In your README to the best of your knowledge please explain the difference between feature and unit test

## Answer
#### Unit test
Check a single part of the code to make sure it's functioning on it's own.
The outcome of a unit test is binary: either "pass" if the program's behavior is consistent with the recorded expectations, or "fail" otherwise.

#### Feature test
With feature tests, you are testing the application by interacting with it just like a real user would do. 
Feature tests mimic the user’s behavior as much as possible, and thats why they are using a web browser to do the tests.

________________
## Question 6. 
In your README to the best of your knowledge please explain what expectations in the context of testing are

## Answer
Expectaions is stating what we want to test. epectations it what we expect of a certain feature or function to do, and compares it to what it actually does.
________________
## Question 7. 
In your README to the best of your knowledge please write a line to line explanation of what is happening in this code

```
<script src="src/js/fizz-buzz.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            let button = document.getElementById('button')
            let displayDiv = document.getElementById('display_answer')
            button.addEventListener('click', () =>{
                let value = document.getElementById('value').value
                let fizzBuzz = new FizzBuzz
                let result = fizzBuzz.check(value)
                displayDiv.innerHTML = result;
            })
        })
    </script>
```
## Answer
`<script src="src/js/fizz-buzz.js"></script>`
Implements script to the HTML file. The script is linked from this source: src/js/fizz-buzz.js.

`<script>`
Opens the script tag in the HTML file.

`document.addEventListener('DOMContentLoaded', () => {`
Adds an event listener that runs when the page has been loaded.

`let button = document.getElementById('button')`
Declare variable button, and the getElementById() method returns the element that has the ID attribute button.

`let displayDiv = document.getElementById('display_answer')`
Declare variable displayDiv, and the getElementById() method returns the element that has the ID attribute display_answer.

`button.addEventListener('click', () =>{`
Creates a click event to a the button variable. It's waiting for a 'click', and once the button is clicked on it will run the code inside.

`let value = document.getElementById('value').value`
Declare variable value, and the getElementById() method returns the element that has the ID attribute value.

`let fizzBuzz = new FizzBuzz`
Declare variable fizzBuzz and assigns it.

`let result = fizzBuzz.check(value)`
Declare variable result and assigns it the result of calling the check function in fizzBuzz with the value from the input field.

`displayDiv.innerHTML = result;`
Finds the innerHTML of the displayDiv variable ('display_answer') and assign it the result.

`})`
Closing.

`})`
Closing.

`</script>`
Closing the script tag in the HTML file.
________________
## Question 8. 
In your README to the best of your knowledge please explain what a CDN (Content Delivery Network) is?

## Answer
It refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content.