## Analyze the apps funcionality 

As a user, I want  a feature, because of reason

MVP (Minimal Viable Product)

As a user 
- I want to be able to have two players because that is how connect four is played 
- I want to be able to take turns
- I want to alternate dropping colored discs into one of seven colums
- I want to be able to win if i get four ina row 
- I want to know who won or if it was a tie 
- I want to be able to play game again if its over 

If I have time I would like to add these if I have time
- Sucess animation
- Dropping Animation
- difficulty setting
- I want to chose my color of my disc 
- keep track of total wins and loses

## Think about the  overall design and look and  feel of the  app

-  clean
- purple and orange for discs
- Font -  Poppins
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Audiowide&family=Londrina+Shadow&family=Poppins:wght@100&display=swap" rel="stylesheet">
```
```css
font-family: 'Poppins', sans-serif;
```

## Wireframe the UI
A wire  frame is a way to represent your game (app) / can have several  wireframes
- High  fidelity
    - Working demo
    - images
    - buttons might be clicakble 
    - hover effects happen
    - little more than just a drawing
- Low fidelity
    - just a drawing
    - layout of the page 
    - where is the header going
    - where are the messages to user going?
    - where are all my buttons going
    - does this feel too crowded or does it feel to empty?

## Pseudocode

-  Define required contants
    - color constant 
- define required variables use to track the state of the game 
    - game board - 1 big array that holds 7 smaller arrays 
- turn - player 1 = 1 || player 2 = -1
- winner - null || 1 || -1 || 'T' for tie
- Cache DOM ELments
    - Message Place that can change 
    - Play Again button
    - column buttons/ markers 
- Upon loading the app should:
    - Init the state vars
        - create the 7 nested arrays 
        - turn var should be set to 1 (player 1)
        - winner var should be null
    - render changes to the DOM
        - render the board, should be compltly blank 
        -render the message purples turn
        - do not render the play again button 
    - wait for interaction 

- Handle a paley clicking a column button
    - update the board array with the player move
    - update the turn var
    -check for a winner
    - re render the board with the players move

- Handle the a player clicking the replay button
    - reset the state var
    - re render the board

- check for a winner
    - check for four in a row
    - we will use offSets to count the colors of the discs in the arrays

## Identify the application's state (data) 

- game board - array of 7 nested arrays
```js
let board
```



