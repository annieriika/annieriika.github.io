---
layout: default
---
## Week 1, Introduction

In the first week we set up our command-line environment. On the command line, we learned to do basic commands such as listing the contents of the current directory, changing the directory, creating, and removing files and directories, copying renaming and moving files, using a text editor, and downloading contents from the internet using `wget`.

Below is a table of basic commands from a Linux command cheat sheet compiled by Alvin Khoo.

| Basic Commands |
| ------ |
| \| | pipe (redirect) output |
| sudo [command] | run <command> in superuser mode |
| nohup [command] | run <command> immune to hangup signal |
| man [command] | display help pages of <command> |
| [command] & | run <command> and send task to background |
| >>[fileA] | append to fileA, preserving existing contents |
| >[fileA] | output to fileA, overwriting contents |
| echo -n | display a line of text |
| xargs | build command line from previous output |
| 1>2& | redirect stdout to stderr |
| fg %N | go to task N |
| jobs | list task |
| ctrl -z | suspend current task |

## Week 2, Navigating a UNIX System

In the second week we learned more about how to navigate the command-line environment. We learned new commands such as copying, moving, and deleting directories, we visited the root directory, learned to compress files and directories,  changing permissions for a file, learning about processes, and connecting to a remote server.

We used the `tar -czvf newfile.tgz oldfile/` command to compress a directory.  

## Week 3, Basic corpus processing

In the third week we learned to do basic corpus processing. We learned about different character encodings, how to change character encodings, converting Windows text files into UNIX text files and vice versa, how to process a text in command line, how to search for patterns, and finally to save the results as a new file.

The command `dos2unix book.txt` transforms a Windows file book.txt into UNIX format.

## Week 4, Advanced corpus processing

In week 4 we learned how to use sed for advanced corpus processing. We learned how to:

*  delete lines from a file using sed
*  find and replace patterns from a file using sed
*  use regular expressions with sed

In addition, we used grep for finding patterns, generated a frequency list from a text file, a sentence per line format and transformed a text into a list of word n-grams.

For example, the command `cat life_of_bee.freq | grep " 27 " | wc -l` finds all tokens that occur exactly 27 times from a Life of Bee frequency list.

## Week 5, Scripting and Configuration Files

In week 5 we learned to write simple scripts. We learned to access command line parameters in scripts, used the if statement in scripts and used echo to see the values of existing environment variables. I used the .bashrc file to make my prompt pretty by changing the colours.

The command `$ chmod u+x myscript.sh` solves a "Permission denied" error while running a script by granting execute permissions.

## Week 6, Installing and Running Programs

In week 6 we learned how to install and run programs on the command line. We learned to give commands as the root user using sudo, installing shoftware using the commands apt-get and brew, installed python packages using pip, created a python virtual environment, and learned to write a Makefile and run it.

In apt-get, you can search for a package using the command: `sudo apt-cache search <keyword>`

Below is a humorous photo of a shell script of a "universal install script".
<img src="assets/images/week6.png" alt="Photo" hspace="20" width="30%" align="center"/>

## Week 7, Version Control

In week 7 we learned to use Github for personal and shared projects. We learned why it’s important, set up a repository, cloned it to our local computer, learned the workflow of adding files, committing changes, and pushing them to the global repository. We also learned how to undo these changes and how to use branches.

The command `git commit -m "your message"`commits the changes to GitHub, and the message should include a short description of the changes.  

## Jekyll and GitHub pages

In the final week we learned how to create Github pages using Jekyll. We installed Jekyll and downloaded webpage templates and created our own page using one of the templates. We learned how to add text, headers, photos, links and code to the page.

The command `bundle exec jekyll serve` builds a local site where you can check that everything is working as it should.