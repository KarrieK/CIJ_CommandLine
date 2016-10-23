#Introduction to the command line#

You have read in files, wrangled data and plotted some graphs in Rstudio but now we're going to teach you how you can leave the Rstudio environment and learn a bit about running scripts in your operating system. 

To do this, we're going to introduce you to the command line and show you how to access, navigate and modify files and folders without using a mouse. 

The advantage of using the command line is its power. You can run programs, write scripts to automate common tasks, and combine simple commands to handle difficult tasks - making it an important programming tool.

##What is the command line?##

The command line is an interface or interpreter that allows us to instruct the computer by typing commands directly to a computer's operating system. It allows us to navigate folders, called directories in the filesystem and perform tasks without using the mouse.

If you run OSx or a Linux based operating system then you are in luck, the command line is going to be your best friend. 
The bad news is that if you run Microsoft Windows your life is going to be a lot tougher. Windows is hostile to developers and not a comfortable environment to code in. 

##How do we access the command line?##

We interact with the command line from a terminal in Linux or OSX or if you are running a windows machine we're going to use a virtual terminal that we'll run from the browser. First create an account on Python Anywhere. 

In OSX or Linux we're going to need to install iterm, which is just a nice terminal.

##Getting started##

Ok first thing's first. Open up your terminal and take a look. There should be some text at the top of the terminal saying something like this:

`Last login: Fri Oct 21 13:32:59 on ttys005
Karries-MacBook:~ karrie$`

The dollar sign $ is called a shell prompt, it's where we're going to input commands.

Well we are now speaking to the operating system but we need to know where we are on that system. 

To do that we are going to use the following command:
* `pwd` - stands for print working directory. This will tell us where we are within the file system

The terminal tells me i'm at `/Users/karrie` - this is the root directory. Contained within this directory are smaller directories like Desktop, Downloads etc...

So we know where we're at but what is in our root directory?
* `ls` - is short for list. We are now asking the machine to list all the contents of that directory

Our terminal lists lots of files and directories but how do we know which is which? The simple answer is to look for a file extenion. If the name has an extension at all like .py, .R or .csv then it's a file or a script. If there is not extension at all then it is a directory and we can move into it.

So I want to see what's in my desktop - to do that I have to navigate into that directory. 

*`cd` - change directory. This command allows us to move into a chosen directory so our command should look like this:

`$ cd Desktop`

Now we are in Desktop and want to look at the work we did today in class. We need to move into the correct folder containing our coursework. 

But are we in the correct place? Check with the pwd command

If we want to move back one folder we can do so easily using `cd ..`




##
