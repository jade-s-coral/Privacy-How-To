# Sources
https://reintech.io/blog/configuring-luks-encrypted-disk-debian-12

# Notes


# Creating a Password
Create a password. I recomend using the "Diceware" approach for password generation. Use a world list of at least several thousand words, the more the better. 
Randomly select 2-3 words from the list to create a passphrase. Sprinkle in randomly selected numbers and special characters inbetween. 
You can roll for multiple words until you can construct a phrase you find somewhat memorable. You are trying to balance keeping your selections as random as possible, but still a phrase you will remember.

There are several large word lists online. Here are a few: https://gist.github.com/atoponce/95c4f36f2bc12ec13242a3ccc55023af
Printer Friendly versions also exist: https://github.com/yannisf/diceware/blob/master/dicewarewordlist.pdf

There are lots of ways to randomly select the words. One method would be to open the word list in a text editor with line numbers, take a 10 sided die and roll for each digit.
For the most significant digit (the far leftmost one) select a dice that divides evenly into that number plus one, roll, divide the result, and take the remainder.
So say for a word list with 279936 words:
* For the most significant digit, 2, I'm picking a 6 sided die because 3 divides into easily and 6 sided die are easy to find.
* Divide the result by 3 and take the remainder. So your results would look like this:
Roll: 1   Remainder: 1
Roll: 2   Remainder: 2
Roll: 3   Remainder: 0
Roll: 4   Remainder: 1
Roll: 5   Remainder: 2
Roll: 6   Remainder: 0
This will make sure you randomly select a digit without weighing your selection towards any numbers.
Then, roll a 10 sided die 5 more times.


