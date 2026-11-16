# Survey Feedback Analyzer

This is my Module End Assignment 4 for Python Fundamentals. It's a small program that reads survey feedback, cleans it up, and tells us a few useful things about it.

## What it does

- Starts with 10 feedbacks that were already given in the assignment
- Lets the user add more feedbacks (name, feedback text and a rating from 1 to 5)
- Cleans the text by removing punctuation, extra spaces and capital letters
- Counts how many feedbacks have the words "good", "poor" and "excellent"
- Shows the average rating, the longest feedback and all the unique words used
- (Bonus) Sorts the feedbacks from highest rating to lowest

## How to run it

1. Open Google Colab and upload `Survey_Feedback_Analyzer.ipynb`
2. Run the cells one by one from top to bottom (Shift + Enter)
3. In Step 2 a box will appear asking for input. Type your answer and press Enter. Type `0` if you don't want to add anything

## How I did it

**Step 1:** I stored the data in a dictionary of lists, exactly as given.

**Step 2:** I used a `while` loop to keep asking until the user types a valid rating between 1 and 5. The serial number goes up automatically starting from 11.

**Step 3:** I wrote a `clean_text()` function. It removes punctuation using `.replace()`, converts to lowercase, and uses `.split()` and `' '.join()` to fix the spaces.

**Step 4:** I wrote `count_word_in_feedbacks(word)`. It checks each feedback and counts it once if the word is there, no matter if it's capital or small letters.

**Step 5:** I used loops to find the average rating, the longest feedback (by number of words) and the unique words. The optional sorting part uses `zip()` and `sorted()`.

## Things I learned

- Working with dictionaries and lists together
- Using loops and if conditions to check user input
- Cleaning text with string methods
- Writing my own functions

## Sample output (with only the original 10 feedbacks)

- "good" appears in 3 feedbacks
- "poor" appears in 2 feedbacks
- "excellent" appears in 1 feedback

## Tools used

Python 3 and Google Colab
