0. Hello World : Write a script that prints “Hello, World”, followed by a new line to the standard output.
+ echo ' Hello, World '

1. Confused smiley : Write a script that displays a confused smiley "(Ôo)'.
+ echo '"(Ôo)'\'

2. Let's display a file : Display the content of the /etc/passwd file.
+ cat /etc/passwd

3. What about 2? :Display the content of /etc/passwd and /etc/hosts
+ cat /etc/passwd  /etc/hosts

4. Last lines of a file : Display the last 10 lines of /etc/passwd
tail -n 10 /etc/passwd
 
5. I'd prefer the first ones actually : Display the first 10 lines of /etc/passwd
+ head -n 10 /etc/passwd

6. Line #2: Write a script that displays the third line of the file iacta.
The file iacta will be in the working directory
You’re not allowed to use sed
+ head -3 iacta | tail -1

7. It is a good file that cuts iron without making a noise :
Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
+ echo ' Best School ' > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)

8. Save current state of directory:
Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
+ ls -la > ls_cwd_content

9. Duplicate last line:
Write a script that duplicates the last line of the file iacta
The file iacta will be in the working directory
+ tail -n 1 iacta >> iacta

10. No more javascript
Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
+ find . -type f  -name "*.js" -delete

11. Don't just count your directories, make your directories count
Write a script that counts the number of directories and sub-directories in the current directory.
The current and parent directories should not be taken into account
Hidden directories should be counted

+ find . -mindepth 1 -type d | wc -l

12. What’s new :Create a script that displays the 10 newest files in the current directory.
Requirements:
One file per line
Sorted from the newest to the oldest
+ ls -t | head

13. Being unique is better than being perfect
Create a script that takes a list of words as input and prints only words that appear exactly once.
Input format: One line, one word
Output format: One line, one word
Words should be sorted
+ sort | uniq -u

14. It must be in that file : Display lines containing the pattern “root” from the file /etc/passwd
+ grep "root" /etc/passwd

15. Count that word : Display the number of lines that contain the pattern “bin” in the file /etc/passwd
+ grep "bin" /etc/passwd | wc -l

16. What's next? :Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.
+ grep -A 'root' /etc/passwd

17. I hate bins: Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
+ grep -v "bin" /etc/passwd | wc -l
