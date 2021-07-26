# Math-Flash-Cards

![Screenshot of Risk-Battle-Simulator](https://github.com/yeri63-hp48g/Math-Flash-Cards/raw/main/Math.png)

Back in the hayday of my youth, I spent the first month of my summer vacation from school learning multiplication tables. At the time I couldn't recall them very quickly, so I was required to spend an hour every day to committing them to memory before going outside to play. This involved memorizing the tables using 3 x 5" index cards, with the equation written on one side, and the answer on the other. I would randomly sort the cards, and attempt to answer from memory, and checking the other side after each attempt. This eventually worked, after many hours of practice.

This program simulates the index card approach for learning addition, subtraction, multiplication and division. It relys on the time needed to answer the question to determine progress. This feedback is shown in the form of a short comment<sup>1</sup> after the equation and answer are revealed, triggered by a button press. The quicker the responce, the more positive the comment. Random equations<sup>2</sup> are shown, starting with 1 + n, where n is any number between 1 and 12. This continues until all 12 equations have been presented, before moving onto 2 + n<sub>2</sub>, 3 + n<sub>3</sub>, etc., to help the student start with the easier tables, and gradually work up to bigger numbers. The order of terms will alternate<sup>3</sup>, so that their memorization is not dependent on a particular order, to recall the answer.

| Table    | Equation Term Order      |
| :-:      | :-:                      |
| Addition | a + b = c<br />b + a = c |
| Subtract | c - a = b                |
| Multiply | a x b = c<br />b x a = c |
| Division | c / a = b                |

The random order of terms are only implemented in addition and multiplication equations. Subtraction and division equations are always presented with the larger term 1st, to avoid generating negative or fractional answers, and unnecessary confusion.

This method of learning works on the honor system, since you could just as well press a button immediately after seeing the equation to reveal the answer. The same is true with the index card approach, by just turning the card over and reading the answer. The program works by asking the student to silently read the equation, and then saying the answer out loud, before pressing the button to validate<sup>4</sup>. Feedback is only provided as an incentive to encourage faster recall, once the basic tables have been learned.

Notes:
1. The feedback comments range from "Amazing!", "Pretty good.", and "Good.", for answers made within 1, 2, and 4 seconds. Anything longer will provoke the "Ok." responce.
2. This program uses the Fischer-Yates shuffle routine to generate the random numbers used to generate the equations. That routine guarantees that no number is repeated, or skipped, which in the end, essentially performs a random sort on the order of equations presented.
3. The order of terms are altered in the following manner, ie. 1 + 5, 8 + 1, 1 + 3, etc., before moving onto the next table. Because only one of the terms is randomly generated, the equations will also change the next time the program is run, ie. 1 + 3, 12 + 1, 1 + 8, etc. This only applies to addition and multiplication.
4. Validation is performed by the student, not the calculator, as it does not have a microphone or speech recognition capabilities. Typing in the answers was considered, but abandoned to focus on developing recall speed instead, the primary goal of this program.
