# Soccer Scorekeeper

## Learning Objectives
- Model out examples of state that might be tracked using an array of objects
- Use an object to create a data model for an item in the human world
- Use the FormData  constructor to grab multiple named values from an HTML form.
- Use the submit handler with e.preventDefault() to manage form submissions.
- Use the type attribute on input tags to create email , number , password , and numerous other inputs.
- Create an object of primitive values and access any item in that object by key using dot and bracket notation
- Create an array of complex values (objects or arrays) and access any item in that array by index using bracket notation
- Describe the difference between val & ref
- Identify what data types are passed by reference vs passed by value
- Write a render function that takes in an object (modeled after a real-world item) and returns a DOM element based on that item.
- Call a render function and append its return value to a grabbed element in the DOM
- Use a for/of loop to loop through an array and for each item, append an element to the DOM using a render function
- Create modular code using import and export with named exports.
- Update multiple pieces of numerical state, each of which can be incremented or decremented on click (i.e, times clicked for multiple buttons).

[Buggy Soccer Scorekeeper](https://github.com/alchemycodelab/buggy-js-soccer-scorekeeper)

### Live Example:
https://alchemycodelab.github.io/web-01-soccer-scorekeeper/


| User should be able to . . .                                                         |             |
| :----------------------------------------------------------------------------------- | ----------: |
| Visit the deployed pages on GitHub pages, with link in the About section of the Github repo|        1 |

| Events                                                                               |             |
| :----------------------------------------------------------------------------------- | ----------: |
| On load, see a form and empty current game div                                             |        1 |
| On submit, add the team names to the current game div.  Call `displayCurrentGameEl` to do this DOM work                                   |        1 |
| On clicking add or subtract, increment and decrement the correct score in the current game div. Call `displayCurrentGameEl` to do this DOM work |     1 |
| On clicking finish, empty the current game div and add the current game to the "past games" div. All past games should be visible in this div. Call `displayAllGames` to do this DOM work. |2|

| Functions                                                              |             |
| :----------------------------------------------------------------------------------- | ----------: |
| IMPURE: `displayCurrentGameEl()` | 2|
| IMPURE: `displayAllGames()` : clears out and appends to games div |2|



*** The Master Plan:

- draw wireframe
- review HTML code to make sure I have all the pieces
- ACP
- Walk through the commented steps in app.js:
    // create an array to hold on to the state of past games

    // get the name data from the form
    // set the state to this data from the form
    // reset the form values
    // refresh the current game element with new data by calling the appropriate function

    // increment the current state for team one's score
    // refresh the current game element with new data by calling the appropriate function

     // increment the current state for team two's score
    // refresh the current game element with new data by calling the appropriate function

    // decrement the current state for team one's score
    // refresh the current game element with new data by calling the appropriate function

     // decrement the current state for team two's score
    // refresh the current game element with new data by calling the appropriate function

     // add the current game to an array of games in state
    // it will be helpful to keep track of these games as objects with 4 properties, one for each piece of state we're tracking
    // for example, make an object like this: { name1: 'ducks', name2: 'bears' ,score1: 1, score2: 2 } 
    // then push it to your array in state
    // (be sure to make a new object. do not declare the object in global scope and mutate it for reuse. This would cause difficult bugs)

    // reset the state to zero and empty strings
    // refresh the current game element with new data by calling the appropriate function
    
    // const gameEl = . . . 
    // make a new gameEl here by calling renderGame with the approriate arguments. 
    // Check the renderGame function declaration in render-utils.js to figure out the correct arguments to pass to this function 
    // In render-utils.js as yourself: How many arguments does the function take? What order does it take them in?

    // clear out the past games list in the DOM

    // loop through the past games in state
    // use the renderGame function to render and append a past game for each past game in state
    // again, review the renderGame function in render-utils.js. How many arguments does it take? What order does it take them in?


- grab any remaining DOM elements
- ACP
- add event listeners
- ACP
