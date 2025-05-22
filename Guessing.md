```mermaid
flowchart TD
    Start([Start]) --> A[The computer randomly chooses a whole number between 1 and 10.]
    A --> B[Ask the participant to guess a whole number between 1 and 10.]
    B --> C[Validate that the input is a whole number between 1 and 10.]
    C -- if input was invalid --> D[Please input a whole number between 1 and 10. Fractions, decimals, and non-number characters such as letters and symbols are not accepted. Please try again.]
    C -- if input was valid --> E[Check if guessed number matches the generated number.]
    E -- if number was correct --> F[Congratulations! You have guessed the correct number.]
    E -- if number was incorrect --> G[Check if guessed number was higher or lower than the randomly generated number.]
    G -- if number was higher --> H[Your guess was too high. Please try again.]
    G -- if number was lower --> I[Your guess was too low. Please try again.]
    F --> End([End])
    H --> B
    I --> B
    D --> B
```
### Steps taken:
1. The computer selects a random whole number between 1 and 10.
2. The participant is asked to guess the number.
3. The computer validates that the input was a whole number between 1 and 10.
4. If the input was invalid, the participant is told to only guess whole numbers between 1 and 10, then sent back to step 2 to guess again.
5. If the input was valid, the computer checks to see if the guessed number was correct.
6. If the guessed number was correct, the participant is congratulated on their correct guess and the game ends.
7. If the guessed number was incorrect, the participant is told whether the guessed number was higher or lower than the randomly generated number, and then is sent back to step 2 to guess again.

