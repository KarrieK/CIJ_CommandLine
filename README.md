#Introduction to the command line#

You have read in files, wrangled data and plotted some graphs in Rstudio but now we're going to teach you how you can leave the Rstudio environment and learn a bit about how you can harness the mighty power of the command line. 

##Why the command line?##
* manage files and folders
* fast and powerful
* automate tasks
* version control - push scripts to your github
* changes the way you think about computing
* sanity check your data

##What is the command line?##

The command line is an interface or interpreter that allows us to instruct the computer by typing commands directly to a computer's operating system. It allows us to navigate folders, called directories in the filesystem and perform tasks without using the mouse.

If you run OSx or a Linux based operating system then you are in luck, the command line is going to be your best friend. 
The bad news is that if you run Microsoft Windows your life is going to be a lot tougher. Windows is hostile to developers and not a comfortable environment to code in. 

##How do we access the command line?##

We interact with the command line from a terminal in Linux or OSX or if you are running a windows machine we're going to use a virtual terminal that we'll run from the browser. First create an account on Python Anywhere. 

##What do you need?##

* OS X - If you're running OS X then you need to install iterm from the apple store
* Linux - No need to do anything, terminals are built into the operating system.
* Windows - You're in a spot of bother, Windows is developer hostile and it's probably best if you just follow along in class

##Getting started##

Ok first thing's first. Open up your terminal and take a look. There should be some text at the top of the terminal saying something like this:

`Last login: Fri Oct 21 13:32:59 on ttys005
Karries-MacBook:~ karrie$`

The dollar sign $ is called a shell prompt, it's where we're going to input commands.

Well we are now speaking to the operating system but we need to know where we are on that system. 

To do that we are going to use the following command:
* `pwd` - stands for print working directory. This will tell us where we are within the file system

The terminal tells me i'm at `/Users/karrie` - this is the home directory. Contained within this directory are smaller directories like Desktop, Downloads etc...

So we know where we're at but what is in our home directory?
* `ls` - is short for list. We are now asking the machine to list all the contents of that directory

Our terminal lists lots of files and directories but how do we know which is which? The simple answer is to look for a file extenion. If the name has an extension at all like .py, .R or .csv then it's a file or a script. If there is not extension at all then it is a directory and we can move into it.

* `ls -a` - reveals hidden files so you see the full contents of your directory
* `ls -t` - sorts files in order of newest first

So I now I know what's in my home directory but I want to move into my desktop so I can se what's in there - to do that I have to navigate into that directory. 

* `cd` - change directory. This command allows us to move into a chosen directory so our command should look like this:

`$ cd Desktop`

Now we are in Desktop and want to look at the work we did today in class. We need to move into the correct folder containing our coursework. 

But are we in the correct place? Check with the `pwd` command

* `pwd` - stands for print working directory

If we want to move back one directory we can do so easily using `cd ..` or two directories `cd ../..`

Ok so maybe we want to move some of our files into a new directory. Let's make that new directory first

* `mkdir` - make directory. This command makes a new directory in the filesystem at the location you have navigated to

Let's create a new directory and call it 'command_line':

`$ mkdir command_line`

What command will tell us if that worked?

Let's move into that directory.

##Moving forward##

We are in our new directory so what now?

Hopefully you grabbed the two files in the repo and they are downloaded onto your machines. Well I think we should take both those files and move them into the our new directory. 

```
$ cd ../..
$ pwd
$ cd Downloads
$ ls
```
See your files? Oh good now let's move them using the `mv` or move command. 

`$ mv NAMES1.csv NAMES2.csv /Users/karrie/Desktop/command_line`

Now take a look, did it work?

Let's read in those files into the termianl to see what's in them. To do that we're going to use `cat`.

So let's try `cat NAMES1.csv`

What have we got?

##Data wrangling##

Now we can read the contents of the csv in the terminal let's dig a little deeper and get some basic information about our data. 

To do that we're going to use a neat little library call csvkit. Let's grab it and install it quickly

`pip install csvkit`

Let's take a look at our csv again to make sure everything is running smoothly. 
`$ csvlook NAMES1.csv`

Let's grab some basic stats about our data to make sure that it matches our csv in R. 
`csvstat NAMES1.csv`




##Where's my stuff?##

There is an amazing find command that will help you find your scripts if you lose them on your file system. 
* `find {file-name}`
You can also look for -type and -name

grep "{search-term}"
http://snugug.github.io/Intro-Command-Line


*csvcut -n data.csv
*csvjoin -c fips data.csv acs2012_5yr_population.csv > joined.csv
*csvstack
*csvmatch

https://github.com/clarkgrubb/data-tools

##Other unix commands##
* `touch` - creates a new text files
* `nano` - allows you to edit a text file
* `cp` - copies a file or directory
* `rm` - removes a file or directory
* `man` - gives you the manual for a command
* `rmdir {folder-name}` - removes an empty directory
* `grep` 

##Resources

If you want to dig deeper and get to know csvkit better then check out the great documentation and tutorial on readthedocs. 

* https://csvkit.readthedocs.org/en/0.9.1/tutorial.html
* https://source.opennews.org/en-US/articles/eleven-awesome-things-you-can-do-csvkit/
* https://www.techonthenet.com/unix/basic/


##Contact me

Email: karrie.anne.kehoe@gmail.com
Twitter: @karriekehoe




##
