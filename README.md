# Math-Flash-Cards

![Screenshot of Risk-Battle-Simulator](https://github.com/yeri63-hp48g/Math-Flash-Cards/raw/main/Math.png)

Back in the hayday of my youth, I spent the first month of my summer vacation from school learning multiplication tables. At the time I couldn't recall them very quickly, so I was required spend an hour every day to committing them to memory before going outside to play. This involved memorizing the tables using 3 x 5" index cards, with the equation written on one side, and the answer on the other. I would randomly sort the cards<sup>1</sup>, and attempt to answer from memory, and checking the other side after each attempt. This eventually worked, after many hours of practice.

This program simulates the index card approach for learning addition, subtraction, multiplication and division. It relys on the time needed to answer the question to determine progress. This feedback is shown in the form of a short comment<sup>2</sup> after the equation and the answer are revealed, triggered by a button press. The quicker the responce, the more positive the comment. Random equations are shown, starting with 1 + n, where n is any number between 1 and 12, followed by 2 + n, 3 + n, and so on, to help the student start with the easer tables, and gradually work up to bigger numbers. The order of the terms will alternate<sup>3</sup>, so that their memorization is not dependent on a particular order of the terms.

| Table    | Equation Term Order      |
| :-:      | :-:                      |
| Addition | a + b = c<br />b + a = c |
| Subtract | c - a = b                |
| Multiply | a x b = c<br />b x a = c |
| Division | c / a = b                |

The random order of terms works well for addition and multiplication, but not so much with subtraction and division. The later two will always need to present the equations with the larger term 1st, to avoid creating equations with negative or fractional results, adding even more confusion.

This method of learning works on the honor system, since you could just as well press a button immediately after seeing the equation to reveal the answer. The same is true with the index card approach, by just turning the card over and reading the answer. The program only works by asking the student to read the equation, and then saying the answer out loud before pressing the button to validate. Feedback was only added as an incentive to encourage faster recall, once the basic tables have been learned.

Notes:
1. This program uses the Fischer-Yates shuffle routine to generate the random numbers used to generate the formulas. That routine guarantees that no number is repeated, or skipped, which in the end essentially performs a random sort of all the equations.
2. The feedback comments range from "Amazing!", "Pretty good.", and "Good.", for answers made within 1, 2, and 4 seconds. Anything longer will provoke the "Ok." responce.
3. Term order is altered in the following manner, ie. 1 + 5, 8 + 1, 1 + 3, etc. Because only one of the terms is randomly generated, the equations will change the next time the program is run, ie. 1 + 3, 12 + 1, 1 + 8, etc. This continues until the ones tables has been completed, before moving onto the twos tables, and so on.
