# Tic-Tac-Toe_project_using_Python
A simple program which pretends to play tic-tac-toe with the user. To make it all easier for you, we've decided to simplify the game. Here are our assumptions:
<ol>
  <li>The computer (i.e., your program) should play the game using 'X's.</li>
  <li>The user (e.g., you) should play the game using 'O's.</li>
  <li>The first move belongs to the computer − it always puts its first 'X' in the middle of the board.</li>
  <li>All the squares are numbered row by row starting with 1 (see the example session below for reference)</li>
  <li>The user inputs their move by entering the number of the square they choose − the number must be valid, i.e., it must be an integer, it must be greater than 0 and less than 10, and it cannot point to a field which is already occupied.</li>
  <li>The program checks if the game is over − there are four possible verdicts: the game should continue, the game ends with a tie, you win, or the computer wins.</li>
  <li>The computer responds with its move and the check is repeated.</li>
  <li>Don't implement any form of artificial intelligence − a random field choice made by the computer is good enough for the game.</li>
</ol>
The example session with the program may look as follows:<br>

+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;1&emsp;&ensp;|&emsp;&ensp;2&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;4&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;6&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;8&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
Enter your move: 1<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;2&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;4&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;6&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;8&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;4&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;6&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;8&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
Enter your move: 8<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;4&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;6&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;4&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
Enter your move: 4<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;3&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;7&emsp;&ensp;|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
Enter your move: 7<br><br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|&emsp;&ensp;X&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;0&emsp;&ensp;|&emsp;&ensp;9&emsp;&ensp;|<br>
|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|&emsp;&ensp;&nbsp;&emsp;&ensp;&nbsp;|<br>
+-------+-------+-------+<br><br>
You won!<br><br>

Requirements
Implement the following features:

The board should be stored as a three-element list, while each element is another three-element list (the inner lists represent rows) so that all of the squares may be accessed using the following syntax:

"Board[row][column]"
 

Each of the inner list's elements can contain 'O', 'X', or a digit representing the square's number (such a square is considered free)
The board's appearance should be exactly the same as the one presented in the example.
Implement the functions defined for you in the editor.

Drawing a random integer number can be done by utilizing a Python function called randrange(). The example program below shows how to use it (the program prints ten random numbers from 0 to 8).

<b><i>Note:</i> The from-import instruction provides access to the randrange function defined within an external Python module called random.</b>
