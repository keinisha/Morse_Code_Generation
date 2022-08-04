# Morse_Code_Generation
Created a user interactive program, coded in MATLAB, that could generate morse code using text.<br><br>
While making this project basic details of the Morse Code were kept in mind – words will be converted to a series of dashes and dots, after each letter there will be a space to differentiate between letters and spaces will be depicted by a backslash to differentiate between words.<br><br>
The relation between the letters to their dot-dash counterpart was created using the concept of Binary Trees. We start at the root node, making it the start point, on moving to the left we add a dot whereas, moving to the right will give us a dash. Completing the tree in this fashion gives us the tree containing the morse codes for all letters, for example – moving to the left from the root gives us 1 dot (.) which represents the letter E, but, if we move to the right of node E we get a dot and a dash (.-) which represents the letter A. <br><br>
To make the program easier to code we have used the concept of cell arrays and have used 27 statements divided into 4 levels, where level 0 represents the root.
 After the tree is defined, two important parts are next – encoding and decoding.<br><br>
Encoding is used to convert text inserted by the user into Morse Code. This is done by defining a function and using to for loop to check and compare each character in the inserted text to the morse tree we created earlier. After the text has been converted to dashes and dots, it can be presented in audio using sounds of different time intervals. The pause between letters will be shorter than the pause between words so that it can be auditorily clear what the sentence is.<br><br>
For example: My name is Keinisha Joshi => -- -.-- / -. .- -- . / .. ... / -.- . .. -. .. ... .... .- / .--- --- ... .... .. <br><br>
Decoding is used to convert Morse Code inserted by the user to text. This is the reverse of encoding; it is applied by defining a function and using the for loop to check every character and compare it to each Morse Tree level to correspond to the letter. After we have converted the Code to text, we can present it in audio format or speech using the .NET framework. <br><br>
Hence the program has the following 
-	Converting Morse Code to Text
-	Converting Text to Morse Code
-	Converting text to Speech
-	Converting Morse Code to Audio
