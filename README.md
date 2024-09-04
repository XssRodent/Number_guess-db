Build a Number Guessing Game
This project, required for your freeCodeCamp certification, involves creating a Bash script for a number guessing game with user information stored in a PostgreSQL database.

Instructions

Project Setup

Create a folder named number_guessing_game within your project directory.

Inside the number_guessing_game folder, create a file named number_guess.sh.

Initialize a git repository in the number_guessing_game folder:

Bash
cd number_guessing_game
git init
Use code with caution.

Script Development

Add a shebang line at the beginning of number_guess.sh:

Bash
#!/bin/bash
Use code with caution.

Implement the script logic using Bash syntax, including:

Generating a random number between 1 and 1000.
Prompting the user for a username with "Enter your username:".
Connecting to the number_guess database (created in a separate step).
Checking if the username exists and retrieving game history.
Welcoming the user appropriately (existing or new player).
Prompting the user to guess the secret number with "Guess the secret number between 1 and 1000:".
Taking user input and validating it as an integer.
Providing feedback based on the guess (higher/lower) until the secret number is guessed.
Updating the database with the user's guess count and best game.
Displaying a success message with the number of guesses taken.
Handling unexpected user input (non-integer guesses).
Database Management (Separate Step)

Connect to the interactive psql shell: psql --username=freecodecamp --dbname=postgres
Create the number_guess database with appropriate tables and columns to store usernames, games played, and best game statistics.
Git Commits

Regularly commit your code changes with descriptive messages using prefixes like fix:, feat:, refactor:, chore:, or test:.
Ensure at least five commits reflecting progress on functionalities.
Submitting to freeCodeCamp (Follow Specific Instructions)

Once the script functions as expected, dump the database using pg_dump.
Submit the number_guess.sh file and the number_guess.sql file to a public repository on a platform like GitHub.
Follow freeCodeCamp's specific instructions for submitting the project URL.
Additional Tips

Consider using command-line tools for database manipulation if comfortable.
Implement error handling for unexpected database interactions.
Break down complex functionalities into smaller functions for better code organization.
Test your script thoroughly with various scenarios and inputs.
By completing this project, you'll gain experience with Bash scripting, PostgreSQL database interaction, and version control using Git.