# Command Line

The way we communicate with our computers is pretty straight forward, we either click, tap, slide, hover, type and so on. These are simple gestures that we use to comand the computer.
Most operating systems that run on servers, desktops, and laptops provide another way of commanding your computer that many people have never even heard of. It is called the command line interface (or CLI), the command line, or the command prompt. 

## How to use command line

Using the command line is as simple as opening up Terminal (available on Mac and Linux) or iTerm (available on Mac only) on your computer, typing a command and pressing enter. Most commands will return some kind of output. Go ahead and open up Terminal and try typing the following command:

```bash
$ echo "Hello, world!"
```
You should see in your terminal another line printed like this:

```bash
"Hello, world!"
```
These is no magic here, is just a simple way to prove that you can use your computer terminal to command your computer.

## Command Line Intro Snippets

In a desktop environment, like that of OS X, you have windows, menu bars, and the desktop to give context to what you are doing. In the command line, however, the context is solely the file system. In fact, files and directories are what make up the command line. Almost everything you do at the prompt will deal with files. 

### File System Legend
Let's look for a moment at some of the symbols that will help us navigate the command line:

```bash
# The root directory or a separator when listing directories
$ / 
# Current directory (also ./) or the same level
$ . 
# The directory one level up (also ../)
$ ..
# Two levels up
$ ../..
# Your home directory or the directory you are placed in when you log in.
$ ~
# The wildcard of the command line and represents "any characters."
$ *
```

The above symbols can be combined with directory and file names to represent their locations.

### Navigating
Navigating your computer's file system is pretty easy with the help of the File System Legend above, and a few simple commands:

```bash
# Change directory
$ cd 
# List folders and files in the directory
$ ls
# Show the current working directory
$ pwd
```

Now let's try to use what we know so far to navigate to our CFG session folder by only using the command line. 

```bash
$ pwd
$ cd <your_cfg_directory>
$ ls
$ ls *.html
$ ls /
$ cd <some_directory>
$ cd ../..
```

### Creating files and folders
Creating files and folders is as easy as navigating through your filesystem. There are some basic commands that you need to get grasp on really well.

```bash
# Make new directory
$ mkdir session3
# Change to the newly created folder
$ cd session3
# Create an empty file inside session3
$ touch index.html
# Copy index.html into main.html
$ cp index.html main.html
# Move main.html into index.html
$ mv main.html index.html
# To edit a file
$ vim index.html
# To see the contents of a file
$ cat index.html
# Remove one file
$ rm index.html
# Remove all html files
$ rm *.html
```

Now all this command seem pretty straigh forward, but if you feel lost and you are not sure what a command does you have all the documentation available just at 3 letters away: `man` command.

Let's say we want to see if the `ls` command has more options rather than just displaying a list of files. What if I want to see the date when the files was last modified? You just type the following: 

```bash
$ man ls
# If you also want to see more details about the listed files use:
$ ls -la
# If you want to sort them by file size
$ ls -lrs
```

### Conclusion
While it may seem difficult at first, being able to use the command line will empower you as a computer user. Once you've learned the basics of using the comand line, you'll be able to simplify and speed up many tasks that were previously tedious. You can be very precise about how you want your computer to perform certain tasks, or about which pieces of information it should display.

#### Notes
* Understand commands that tutorials tell you to use:

    * As you learn programming, you will inevitably have to use the command line to install software, compile or run code, and perform other types of system administration.
    * Learning the basics of the command line will help you understand why you are running the commands, and give you a general idea of how they work.
    *  The command line, as with all power, has its risks. You have the capability to instruct the computer to do many things. If you instruct the computer to erase all of your data, it will cheerfully proceed to do so. Do not run a command just to see what it does. Make sure you understand what the command is supposed to do first, especially if the command involves changing or removing files.

Being able to communicate with your computer or server via command line gives you immense and precise power over your computer. You can take advantage of a lot of powerful tools in their raw, powerful form.

Happy coding! 

_xoxo Mirela_
