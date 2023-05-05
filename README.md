Download Link: https://assignmentchef.com/product/solved-cse1141-assignment-4
<br>
In this homework, you will write a program which will take an input string, if the word is either “<strong>exit</strong>” or “<strong>quit</strong>”, your program should terminate; if the word is “<strong>stat</strong>”, your program should print a two-line statistical report: the first line prints <em>the total number of words the user has entered</em>, and the second line prints <em>the total number of alphabetic letters</em> the user has entered. Note that we only count the 26 letters in the alphabet. For example, if a user has entered the following string, i.e. “We love CSE1141 course a lot!!”, the following should be printed to screen after the user types “<strong>stat</strong>”:

The number of words: 6

The number of alphabetic letters: 19




If the word is not “<strong>stat</strong>”, “<strong>exit</strong>” or “<strong>quit</strong>”, then your program will ask to change the case of letters, count vowels and consonants, capitalizes the first letter of each word, and encrypt or decrypt the input string based on the user’s selection.




To implement this program, you need to define following methods:

<ul>

 <li><strong>public static void main(String[] args)</strong></li>

</ul>

o add two variables, both of type <strong>int</strong>, to the “main” method to store the total number of words and the total number of letters the user has entered since your program starts. You can create an infinite loop in the “<strong><em>main</em></strong>” method; in each iteration of the loop, first ask the user to enter an input string and then it will ask to select an option. You can invoke related methods based on the option selected.




<ul>

 <li><strong>public static int updateLetterCount(int count, String str) </strong></li>

</ul>

o take as input the current count of the letters and the string the user has just entered. This method updates and <strong><em>returns the new letter count value</em></strong>. This method should be called each time the user enters a new string that is not “<strong>exit</strong>”,

“<strong>quit</strong>”, or “<strong>stat</strong>”.




<ul>

 <li><strong>public static void printStat (int wordCount, int letterCount) </strong>o takes as input the total word count and the total letter count, and prints the above-mentioned two-line statistical report on screen, with <strong><em>no return value</em></strong>.</li>

</ul>




<ul>

 <li><strong>public static String changeCase (String str) </strong></li>

</ul>

o <strong><em>returns a new string</em></strong> in which the uppercase letters are changed to lowercase and lowercase letters are changed to uppercase.




<ul>

 <li><strong>public static void countVC (String str) </strong></li>

</ul>

o displays the number of vowels and consonants in an input string.




<ul>

 <li><strong>public static String capitalize (String str) </strong></li>

</ul>

o takes an input string and<strong><em> returns a new string</em></strong> in which the first letter of each word is capitalized.




<ul>

 <li><strong>public static String encryptOrDecrypt (String str, int offset) </strong>o encodes or decodes input string based on a shift offset.  o The method will take an input string, convert it into uppercase, then process it using the shift offset.</li>

</ul>

o This method will take an integer offset and it will perform encryption if the value is positive and it will perform decryption if it is negative.  o The value of offset must be -25 to -1 (inclusive) and 1 to 25 (inclusive).  o Encoding/decoding scheme is given in the following figure.



















Example run:




Please enter an input string: heLLo worLd

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 1

HEllO WORlD







Please enter an input string: Welcome to JAVA!

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 2

The number of vowels is 6

The number of consonants is 7







Please enter an input string: welcome to marmara university!

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 3 Welcome To Marmara University!







Please enter an input string: We love CSE1141 course a lot!!

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 4

Enter an offset value: 3

Source: WE LOVE CSE1141 COURSE A LOT!!

Processed: ZH ORYH FVH1141 FRXUVH D ORW!!







Please enter an input string: ZH ORYH FVH1141 FRXUVH D ORW!!

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 4

Enter an offset value: -3

Source: ZH ORYH FVH1141 FRXUVH D ORW!!

Processed: WE LOVE CSE1141 COURSE A LOT!!










Please enter an input string: We love CSE1141 course a lot!!

<ol>

 <li>Change Case</li>

 <li>Count vowels and consonants</li>

 <li>Capitalize the first letter</li>

 <li>Encrypt or Decrypt</li>

</ol>




Please select an option: 4

Enter an offset value: -26 Invalid offset.







Please enter an input string: stat

The number of words: 27

The number of alphabetic letters: 106







Please enter an input string: exit

Program ends. Bye





