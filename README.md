Download Link: https://assignmentchef.com/product/solved-program-that-encrypts-the-alphabetic-letters-in-a-file-using-the-vigenere-cipher-in-java
<br>
In this assignment you’ll write a program that encrypts the alphabetic letters in a file using the Vigenère cipher. Your program will take two command line parameters containing the names of the file storing the encryption key and the file to be encrypted. The program must generate output to the console (terminal) screen as specified below.

<strong>Command Line Parameters</strong>

Your program <strong>must</strong> compile and run from the command line.

The program executable must be named “vigenere” (all lower case, no spaces or file

extension).

Input the required file names as command line parameters. Your program may NOT

prompt the user to enter the file names. The <strong>first parameter</strong> must be the name of the encryption key file, as described below. The second <strong>parameter</strong> must be the name of the file to be encrypted, as also described below. The sample run command near the end of this document contains an example of how the parameters will be entered.

Your program should open the two files, echo the processed input to the screen, make the necessary calculations, and then output the ciphertext to the console (terminal) screen in the format described below.

<strong>Note:</strong> If the plaintext file to be encrypted doesn’t have the proper number of alphabetic characters, pad the last block as necessary with the letter ‘X’.

<strong>Encryption Key File Format</strong>

The encryption key is plain text that may contain upper and lower case letters, numbers, and other text. The input must be stripped of all non-alphabetic characters. Please note that the input text must be converted to contiguous lower case letters to simplify the encryption process.

<strong>Format of the File to be Encrypted</strong>

The file to be encrypted can be any valid text file with no more than 512 letters in it. (Thus, it’s safe to store all characters in the file in a character array of size 512, including any padding characters.) Please note that the input text file will also generally have punctuation, numbers, special characters, and whitespace in it, which should be ignored. You should also ignore whether a letter is uppercase or lowercase in the input file. Thus, you should treat ‘A’ and ‘a’ the same in your program. Therefore, convert the upper case letters to lower case letters.

<strong>Output Format</strong>

The program must output the following to the console (terminal) screen:

Echo the input key file

Echo the input plaintext file

Ciphertext output produced from running the cipher against the input plaintext file.

The ciphertext output portion should consist of only lowercase letters in rows of exactly 80 letters per row, except for the last row, which may possibly have fewer. These characters should correspond to the ciphertext produced by encrypting all the letters in the input file. Please note that only the alphabetic letters in the input plaintext file will be encrypted. All other characters should be ignored.

<strong>Program Notes and Hints</strong>

Your program must read in an input plaintext file that may contain uppercase letters, lowercase letters and non-letter characters. Your program must distinguish between these three groups so that only the letters get encrypted. All non-letter characters in the file are simply skipped and not counted as part of the plaintext. Please note that although both upper case and lower case letters will be encrypted, your program should not treat them differently, that is, the program should process an upper case input letter the same as the corresponding lower case letter, i.e., it should treat an ‘A’ the same as an ‘a’.

One possible breakdown to solve this problem is as follows:

1) Write a section of code or function that reads only the upper and lower case letters in the input file into an char array of size 512, storing only the appropriate lowercase letters in the character array.

2) Write a section of code or function that takes as input the array from section 1 and the encryption key and produces an array of ciphertext storing only lowercase letters.

3) Write a section of code or function that takes as input the array storing the ciphertext and outputs it to the screen in the format specified. Additional functions or code will be needed to echo the input key and plaintext files.

<strong>Sample Key File</strong>

<strong>“Computer programming is an art, because it applies accumulated knowledge to the world, because it requires skill and ingenuity, and especially because it produces objects of beauty. A programmer who subconsciously views himself as an artist will enjoy what he does and will do it better.” – Donald Knuth</strong>

<strong>Sample Input File</strong>

<strong>678901234567890123456789012345678901234567890 “Cowards die many times before their deaths; The valiant never taste of death but once. 678901234567890123456789012345678901234567890 Of all the wonders that I yet have heard,</strong>

<strong>It seems to me most strange that men should fear; Seeing that death, a necessary end, 678901234567890123456789012345678901234567890 Will come when it will come.” 678901234567890123456789012345678901234567890</strong>

<strong>―</strong> <strong>William Shakespeare, Julius Caesar</strong>

<strong>Corresponding Output File</strong>

<strong>eciplwwuxvageyfuuryjwfbrvmiikrxwebasiwpdedicpnzygekxdcgskqhhgxapnasjqvzibpntbwaw guihmbyelaimesaihprgvqcblcezvxgbiowsedrsepgyllimbvbvbqydrgnetlwsnoktbtrdtrhnrnqo ijohfqyofkvdnkcgwhfzvmpoptxusxjwalyirfaztgmdainashqsinzgdswsrkatfiialfqybqqboalk xiahkrqe</strong>