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

*`cd` - change directory. This command allows us to move into a chosen directory so our command should look like this:

`$ cd Desktop`

Now we are in Desktop and want to look at the work we did today in class. We need to move into the correct folder containing our coursework. 

But are we in the correct place? Check with the `pwd` command

* `pwd` - stands for print working directory

If we want to move back one directory we can do so easily using `cd ..` or two directories `cd ../..`

Ok so maybe we want to move some of our files into a new directory. Let's make that new directory first

*`mkdir` - make directory. This command makes a new directory in the filesystem at the location you have navigated to

Let's create a new directory and call it command_line:

`$ mkdir command_line`

What command will tell us if that worked?

'ls' will let us know if we successfully created a new directory. 

So let's move into that directory.

##Moving forward##

Let's make a note to ourselves and remind us 

* `touch` - creates a new text file 
* `nano` - lets you edit a text vile
* cp
rm
mv 
man
rmdir {folder-name} - removing empty directory


The cp command copies files or directories. Here, we copy the contents of x.txt into y.txt.

mv superman.txt superhero/

rm --help

echo "{content}" >: Will write content to a file
cat: Will preview content in a file

##Where's my stuff?##

There is an amazing find command that will help you find your scripts if you lose them on your file system. 
* `find {file-name}`
You can also look for -type and -name

grep "{search-term}"
http://snugug.github.io/Intro-Command-Line

*csvclean
*csvstat
*csvcut -n data.csv
*csvjoin -c fips data.csv acs2012_5yr_population.csv > joined.csv
*csvstack

https://github.com/clarkgrubb/data-tools






##
