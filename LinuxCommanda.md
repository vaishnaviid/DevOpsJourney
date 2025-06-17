# Linux Commands

To start practice commands on aws:
1. create EC2i instance
   
2. Use the ssh command with your .pem key file and the public IP of your EC2 instance like this:

    ssh -i /path/to/your-key.pem ec2-user@ec2-public-ip

## Basic Linux Commands
ls → List the files and directories

ls -l → Long listing of all directory files (in alphabetical order)

ls -l dirname → Content inside the directory

ls -lr → Reverse alphabetical order

ls -lt → Displays the latest files on top

ls -ltr → Old files on top

ls -la → Displays hidden files

pwd → Present working directory

clear → Clears the terminal

whoami → Username details

date → Day

cal → Date with month calendar

history → Command history

cd dirname → Change directory

cd .. → Go to previous directory

cd ~ → Switch to home directory

mkdir dirname→ Create directory

rmdir dirname → Delete directory if it is empty

rm filename→ Delete file

rm * → Remove all the files in directory

rm -rf dirname → Delete non-empty directory

mv filename newfilename → Rename file

mv filename dirname/filename → Move file from one location to another

touch filename→ Create empty files

cat > filename → Create and add content

cat >> filename → Append data

cat filename → Print file content

cat file_1 file_2 > file_3 → Copy more than one file data into another file

cat -n filename → Print data with line numbers

tac filename →Print file data from bottom to top

rev filename → Reverses each line of data

cp fileone filetwo → Copy file data from one to another

wc filename→ Word count (no of lines, words, chars)

cmp fileone filetwo → Compare files

diff fileone filetwo→ Check differences

head filename → Prints only first 10 lines(default) from the file

head -n 5 filename → Print 5 lines from top

tail filename→ prints the last 10 lines from the file

tail -n 5 filename → Print 5 lines from the bottom

tail -f filename → Get the live data (newly added)

grep 'word' filename → Global regular expression print → case sensitive command

grep -i 'word' filename → Search a word (except case sensitivity)

grep -i 'word' * → Searches the word in all the files

grep -n 'word' filename → Print lines having word with line number

grep -v 'word' filename → Skips the line containing that word & prints all other content from the file

NOTE : We can use a combination of any option.

vi filename→ visual editor, can create and modify file data → Three Modes → command mode (open file) → insert mode (press i) → exit mode (esc + :wq! (to save), esc + q!(unsave and exit))

nano filename→ create file and add data into it → Two Modes → command mode (just open file) → exit mode (ctrl + x + y(to save), ctrl + x + n(unsave and exit))

sed → Stream editor, used to substitute, modify and delete the data

sed 's/word1/word2/' filename → Change /replace first occurance of word

sed 's/word1/word2/2' filename → Change /replace second occurance of word

sed 's/word1/word2/g' filename → Change /replace all of occurrences of word with the second

sed -i 's/word1/word2/g' filename → Save changes permanently

sed '4d' filename → Delete line

sed '$d' filename → Delete last line

sed '3, $d' filename → Delete 3rd to last line

sed -i '4d' filename → Delete line from the file permanently

sed '/word/p' filename → Print line twice containing a word

sed '/word/d' filename → Delete line containing a word

sed -n '3,6p' filename → Print data 3rd line to 6th line

sed '4i/data' filename → Insert a data before 4th line

sed '$a/data' filename → Insert a data after the line

awk → Perform ops on files containing structured data, also called a filter command

awk '/word/ {print}' filename → Print data with certain word in it

awk '{print $3, $7}' filename → Print data from column 3 and 7

awk '{print NR, $0}' filename → Print data with record number

awk '{print NR, $0} filename → Print file data with line numbers

awk '{print NR "-" $1} filename → Print first col data with line numbers and -

awk '{print NR "@" $1} filename → Print first col data with line numbers and @

## Conclusion 

These basics are crucial for working confidently on cloud platforms like AWS, where Linux powers most infrastructure.

Stay tuned as I continue exploring Linux in upcoming posts. If you're also following the #90DaysOfDevOpsChallenge, keep practicing.

Let’s keep learning and growing together!
