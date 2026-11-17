
# AIXcelerate - Mood Guesser

## 1. Project Overview

A simple Python-based mood prediction program that identifies whether a sentence expresses a Happy or Sad mood using predefined clue words.

## 2. Technologies Used

- Python
- Visual Studio Code
- GitHub

## 3. Project Features

### Level 1 - Count the Moods
- Counts Happy and Sad sentences.
- Uses a for loop and if-else conditions.
- Training dataset contains 15 sentences.

Output:
(8, 7)

### Level 2 - Guess the Mood
- Uses six Happy clue words and six Sad clue words.
- Converts sentences into lowercase.
- Removes punctuation using string replacement.
- Splits sentences into individual words.
- Counts matching clue words.
- Predicts the mood based on the higher score.
- Returns Sad when both scores are equal.

### Level 3 - Testing and Accuracy

Tested using the five official practice sentences.

- Correct predictions: 4
- Incorrect predictions: 1
- Total sentences: 5
- Accuracy: 80%

## 4. Project Reflection

The program incorrectly predicted "Today was a great day" as Sad.

This happened because none of the words in the sentence matched the predefined clue-word lists. Both scores became zero, so the tie-breaking rule returned Sad.

One improvement would be to use a larger and more varied training dataset and improve the clue-word selection.

## 5. Learning Note Answers

1. The total score of "good party today" is +3, so it is Happy.
2. The total score of "bad exam day" is -3, so it is Sad.
3. The word "exam" received zero because it appeared equally in Happy and Sad examples.
4. "Not good" is incorrectly classified because the program ignores negation. It could be improved by detecting words such as "not".

## 6. How to Run

1. Install Python.
2. Open the project folder in VS Code.
3. Open main.py.
4. Run the Python file.

## 7. AI Assistance Acknowledgment

ChatGPT was used as a learning assistant to understand Python concepts, discuss clue-word selection, review code, and troubleshoot errors. The implementation and testing were reviewed during development.

