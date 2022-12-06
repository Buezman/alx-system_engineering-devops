## Shell variables and expansions tasks commands
0. Create a script that creates an alias
```
	alias ls='rm *'
```
1. Create a script that prints hello user, where user is the current Linux user
```
	echo "hello $USER"
``` 
2. Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program
```
	export PATH=$PATH:/action	
```
3. Create a script that counts the number of directories in the PATH.
```
	echo $((`echo $PATH | grep -o ":/" | wc -l`+ 1))
```
4. Create a script that lists environment variables.
```
	printenv
```
5. 5-local_variables - Create a script that lists all local variables and environment variables, and functions
```
	set
```
6. 6-create_local_variable -  Create a script that creates a new global variable (name: BEST, value: School)
```
	BEST=School
```
7. 7-create_global_variable - Create a script that creates a new global variable (name: BEST, value: School)
```
	export BEST=School
```
8. 8-true_knowledge - Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line
```
	echo $((128 + $TRUEKNOWLEDGE))
```
