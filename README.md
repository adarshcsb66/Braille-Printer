# Braille-Printer
Code for Punching of Braille, 
Built a cheap and efficient braille printer as part of a course project.
The printer is cheaper compared to the ones commercially available and also more efficient in printing.
The efficiency of the printer was increased by making it punch while going from left to right and also when returning from right to left.
The code is efficient and occupies only 50% of the memory of the Arduino Uno board.

# Working of the code and algorithm
The whole page was perceived as a 2-D array of size 12 * 20(easily changable because finally variables were used) considering the requirements of the Braille alphabet.When the input was taken the letters and numbers present in the input string were broken down into their respecitve Braille counterparts and the "page" array was made.
Then a for loop was run from 0 to the width of the page(in this case 12 units) and the puncher was activated wherever required by the page array.
After repeating the above step three times(L--->R,R--->L,L--->R),a function "next_line" was called which activated the motors which pushed the page down and then the process begins again.
