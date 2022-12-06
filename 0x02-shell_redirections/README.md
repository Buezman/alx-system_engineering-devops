1. Prints "Hello, World" to the standard output
```
	echo 'Hello, World'
```
2. Prints confused smiley "(Ôo)' to output
```
	echo "\"(Ôo)'"
```
3. Display the content of the /etc/passwd file
```
	cat /etc/passwd
```
4. Display the contents of /etc/passwd and /etc/hosts files
```
	cat /etc/passwd /etc/hosts
```
5. Display the last 10 lines of /etc/passwd file
```
	tail -n 10 /etc/passwd
```
6. Display the first 10 lines of /etc/passwd file
```
	head -n 10 /etc/passwd
```
7. Displays the third line of the file iacta
```
	head -3 iacta | tail +3
``` 
8. Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
```
	echo "Best School" > \\*\\\\'\"Best School\"\\'\\\\\*$\\?\\\*\\\*\\\*\\\*\\\*:)	
```
9. Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
```
	ls -la > ls_cwd_content
```
10. Write a script that duplicates the last line of the file iacta
```
	tail -n 1 iacta > iacta	
```
11. Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
```
	find . -type f -name "*.js" -delete
```
12. Write a script that counts the number of directories and sub-directories in the current directory
```
	find . -type d -not -name '.' | wc -l
```
13. Create a script that displays the 10 newest files in the current directory
```
	ls -t1 | head -n 10
```
14. Create a script that takes a list of words as input and prints only words that appear exactly once
```
	sort | uniq -u
```
15. Display lines containing the pattern “root” from the file /etc/passwd
```
	 cat /etc/passws | grep 'root'
```
16. Display the number of lines that contain the pattern “bin” in the file /etc/passwd
```
	grep -i 'bin' /etc/passwd | wc -l	
``` 
17. Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd
```
	grep -i 'root' -A 3 /etc/passwd
```		
18. Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
```
	grep -i '^bin' /etc/passwd
```
