## Problem

- Build six squares with no color.
- Every time you click one, it turns green.
- When the last square turns green, they all go back to no color in backwards sequence to which it was clicked (not all at once)

## Resolve

1. Creating the six squares
2. Determining a way to change their color when clicked
3. Create a mechanism to track which squares have been clicked
4. Devise a method for the squares to return to their original state in the reverse order they were clicked

## Process

1. step 1: creating the six squares
    - CREATE six individual buttons in HTML 
    - GIVE each button a class name of square
    - GIVE them unique IDs

2. step 2: Determining a way to change their color when clicked

    - ADD a CLICK Event Listener to each button
    - CALL a function called UpdateSquares() that changes the color of a clicked button

3. step 3: Create a mechanism to track which squares have been clicked

    - CREATE an array called `array_sqr` that stores the unique ID of a clicked button
    - When a button has been clicked, add the ID to the array

4. step 4: devise a method for the squares to return to their original state in the reverse order they were clicked

    - When `array_sqr.length == 6` call a function called ReverseSquares()
    - In the ReverseSquares() function, loop through `array_sqr`
    - Inside the loop, SELECT each button with the unique IDs in `array_sqr`
    - REMOVE the color green from the selected button


## Reference
[Main Reference](https://www.freecodecamp.org/news/how-to-build-projects-as-a-junior-developer/)