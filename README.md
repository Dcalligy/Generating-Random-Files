# Generating Random Quiz Files
This comes from the book Automate The Boring Stuff With Python (page 186). The problem ask the following: 

Say you're a geography teacher with 35 students in your class and want to give a pop quiz on US state capitals. Alas, your class has a few bad eggs in it, and you can't trust the students not to cheat. You'd like to randomize the order of questions so that each quiz is unique, making it impossible for anyonw to crib answers from anyone else. Of course, doing this by hand would be a lengthy and boring affair. Fortunately, you know some Python.

Here's what the program does:

* Creates 35 different quizzes.
* Creates 50 multiple-choice questions for each quiz, in random order.
* Provides the correct answer and three random wrong answers for each question, in random order.
* Writes the quizzes to 35 text files.
* Writes the answer keys to 35 text files.

This means the code will need to do the following:

* Store the states and their capitals in a dictionary.
* Call ```open()```, ```write()```, and ```close()``` for the quiz answer key text files.
* Use ```random.shuffle()``` to randomize the order of the questions and multiple-choice options.
