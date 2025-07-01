- to check the active shell
```
echo $SHELL
```
- to know what to enter to change to bash 
```
which bash
```
```
```
- .sh is extension(but not necessary)
- have to make the script executable
```
  sudo chmod u+x
```
- In ubuntu by default the executable show the files in green
- **"#!/bin/bash"** at the beginning of a bash script is called a ==**shebang**== or **==hashbang==**
# Variables
```
myname = "Chinmay"
```
- referencing it
	1. echo ==$==myname
	- have to include ($)dollar sign in front of my name var


> [!Important] Single Quote(' ') v/s (" ")
> When we  do single quote shell prints the content without paring the variables wheweras during "" it interprets the variables 

eg. 
```
echo "Hello my name is $name"
>Hello my name is Chinmay

echo 'Hello my name is $name'
>Hello my name is $name
```

![[{65452550-96B9-46CC-85C5-FCBAB5E6074C}.png]]
![[{970E4982-D673-4389-AAA9-1CA607C1AF3A}.png]]

---
## Sub Shell
- allows you to execute a command in the background
```
files=$(ls)
echo files
```

## Date
- date >gives the current date and time
```
chinmay@chinmay-VMware-Virtual-Platform:~/Desktop/bash$ date

Mon Mar 24 10:44:49 AM IST 2025
```

## $USER variable

- In linux, default environment variables are predefined key-value pairs that provide essential information about the system and user environment. These variables are automatically set by the system and are available to all processes
- USER is one of them 

> [!NOTE] Best Practive
> The system's environment variables are written in capital letters(eg. $HOME)
> and user defined ones are in small letter


- to list the environment variables

```bash
printenv
or 
env
```

