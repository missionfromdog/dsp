# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> >
* mkdir makes a directory
* ../ up one directory
* ../../ up two directories
* touch - create a file
* cat - reads a file
* grep - can't remember
* pip
* rm - removes a file
* pwd - print working directory
* ls - list contents of a directory, (alt)
* open - opens a file
* nano ~/. opens nano environment editor




---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> > 
ls lists all the files in the current directory
ls - a lists all files + the hidden files (denoted with a period (.)
ls - l lists all files (non-hidden) with details about each file (file rights, author, size, date)
ls - lh lists all files, with the h gives 'human readable format' to the file sizes, typically in bytes, kb, mb, etc.
ls - lah combines mentioned above, all + hidden, plus file sizes.
ls - t the 't' sorts the files listed by their last modification date
ls - Glp the G adds color to the output of just the file category.

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> >
ls -1 is very functional;
ls -g great view of a directory w/out the owner; less is more.
ls -d seems very functional to get only directories, i like it.
ls -lt nice list sorted by last modified
ls -1r reverse order in a vertical list; can't get enough -1

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > 
Xargs reads data from the input (that you give it) and executes it based on the argument given.  In laymans terms, it allows you to create and run a short script which can include multiple commands like find and greg within it and return results. 

It can also read a file and execute commands within it and then pass those arguments and pass them to other commands.  I can see how this might be useful for data science to ask Xargs to read a file (a python script or argument) and then send those results to another file.  I'm guessing this might be a nice way to ask an API for data.

 

