# Constructor-Word-Guess
CLI word guessing game.

File Components:

letter.js--

-letter constructor that displays a letter, or a placeholder '?'
        -depending on if the game player has guessed the correct letter
      1. Empty string to store the letters for a random word
      2. Boolean value set to false as the status for the pending guess
      3. Function that returns the correct letter if guessed or a the placeholder '?'
      4. Function that takes a pressed key's value and checks it against the stored correct letterS, and will update the value to true if the letter matches


word.js

-word constructor that creates a word from the letter constructor stored letters
        -file should require letter.js
      1. Array of NEW letter objects for the underlying word
      2. Function that concatenates the letters of the letter.js list item #3 function to display a string
      3. Function that that takes the pressed key's value calls the letter.js list item #4. function 


index.js

-holds the functionality of the game
        -should require word.js
      1. Randomly selects a word from the word bank array and uses the word constructor to store it 
      2. Uses inquire to prompt the user for a new guess and tracks the remaining incorrect guesses left


