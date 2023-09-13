# Quiz-Sample
# 🚀 Code Description:

The provided Python code is for creating a sample quiz program using Object-Oriented Programming (OOP) principles. It imports classes from three different modules (`question_model`, `data`, and `quiz_brain`) to create a quiz and evaluate the user's answers. Here's a breakdown of the code:

1. Imports: The code imports the necessary classes and data from external modules:
   - `Question` class from `question_model.py`
   - `question_data` list from `data.py`
   - `QuizBrain` class from `quiz_brain.py`

2. Question Bank Initialization:
   - A list called `question_bank` is initialized to store instances of the `Question` class.
   - A `for` loop iterates through each dictionary in the `question_data` list.
   - For each dictionary, it extracts the question text and answer and creates a new `Question` object.
   - These `Question` objects are appended to the `question_bank`.

3. Quiz Initialization:
   - An instance of the `QuizBrain` class is created with the `question_bank` as an argument. This initializes the quiz with the provided questions.

4. Quiz Loop:
   - A `while` loop is used to continue the quiz until there are no more questions in the quiz brain (`still_has_question()` method).
   - Inside the loop, the `next_question()` method is called to present the next question to the user.
   - The user's response is not captured in this code but would typically be obtained through user input.

5. Quiz Results:
   - Once all questions are answered (the loop exits), a message is printed to indicate the end of the quiz.
   - The user's final score is displayed using string formatting, showing the number of correct answers out of the total number of questions.

# 🔐 Code Specifications:

- The code imports the `Question` class, `question_data` list, and `QuizBrain` class from separate modules (`question_model`, `data`, and `quiz_brain`), that are correctly imported.

- The code relies on the following methods from the `QuizBrain` class:
  - `still_has_question()`: Determines if there are remaining questions in the quiz.
  - `next_question()`: Presents the next question to the user.

- The final score is displayed using string formatting (`{quiz.score}/{quiz.question_number}`), where `quiz.score` represents the number of correct answers, and `quiz.question_number` represents the total number of questions.

- It's essential to ensure that the provided data in `question_data` matches the expected format, with each question represented as a dictionary with "text" and "answer" keys.
