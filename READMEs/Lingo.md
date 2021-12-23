
# LINGO (C - Shell Scripting) | Fall 2021
- Two different programs, one made entirely out of unix commands (bash) and the other written in C (with use of structs and linked-lists) to play bingo on terminal as the final project of CPS 393 to demonstrate in-depth knowledge of the course material.
- Academic Course: CPS 393 | Grade: 100%
### Contents:
* 🎮  [Game Play]()
* 🚨  [Exit Statuses]()

## 🎮 Game Play:
User runs LINGO with a card (a 5x5 matrix of integers), and the program calls random numbers one-by-one (triggered by any key, except “q” which quits the program). Each time a number is called, if that number appears on the user's card, it is "marked". User wins when a row, or column, or all 4 corners, becomes marked.

Demo of game play:

https://user-images.githubusercontent.com/72219373/147281156-c543ef63-3900-43a9-aded-5f387af40956.mp4

**Note**: the above videos may not show on some browsers. You can watch it [here](https://user-images.githubusercontent.com/72219373/147281156-c543ef63-3900-43a9-aded-5f387af40956.mp4).

### LINGO card structure:
A perfectly formatted LINGO card a seed number (all integers) at the top and then 5 columns of 5 integers, in which the first column contains 5 unique numbers 0-15, second in 16-30, 3rd in 31-45 (with the middle number as “00” and already marked), 4th in 46-60, and the final column in range of 61-75. 
#### Sample LINGO Card:
1063<br>
12&ensp;23&ensp;42&ensp;55&ensp;74<br>
04&ensp;19&ensp;34&ensp;46&ensp;72<br>
07&ensp;17&ensp;00&ensp;51&ensp;69<br>
11&ensp;30&ensp;44&ensp;56&ensp;62<br>
09&ensp;27&ensp;40&ensp;47&ensp;67<br>

### Solo Mode:
- User supplies a LINGO card in a file, whose name is sent as an argument to the program ($1). 
- The program will display the list of called numbers so far followed by the marked card (initially, call list is empty and only 00 is marked), displaying Card with column titles "L", "I", "N", "U", "X".
- User used any key (except "q") to trigger number calls, until they win (5 in a row or column, or all 4 corners being marked) or quit (hitting the "q" key).

### Group Play:
- Two or more players may play with each other by using card files with the same seed number but different card layout. Same seed number guarantees that they will get the same number calls.
- The game play process is the same as solo mode.

## 🚨 Exit Statuses:
1. Card input file doesn't exist, is not readable, etc.:
  	exit 1. "input file missing or unreadable"
2. Card input file does not have exactly 6 lines:
  	exit 2. "input file must have 6 lines"
3. Seed line is incorrect (contains one or more non-digit characters):
  	exit 3. "seed line format error"
4. card has incorrect layout and/or number(s):
  	exit 4. "card format error"
5. If LINGO finishes because user quits prematurely (enters q), or wins:
  	exit 0.

