# 1- The Command Line:

- simply is a text based inteface to the system, you are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text, it typically presents you with a prompt & it will be displayed after the prompt..

- I can't tell you exactly how to do it as every system is different but here are a few places to start looking:

* If you're on a ***Mac*** then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
* If on ***Linux*** then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.
* If you are on ***Windows*** and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .

<br>
<hr>

# 2- Basic Navigation:
 Many tasks rely on being able to get to, or reference the correct location in the system. As such, this stuff really forms the foundation of being able to work effectively in Linux
at first you should know where are you ? (what is your location in files??) use `pwd` then use `cd` to change your dirctory to another.. use `cd..` to go back step forward or use `ls` to know the 'Relative paths' in your dir..

<br>
<hr>

# 3- More About Files:
well there is alot about linux to know & also alot of characteristics like:
- everything is actually a file!
A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc..
- Linux is an Extensionless System!
- Linux is Case Sensitive!

<br>
<hr>

# 4- Manual Pages:
The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. Some of them are a little hard to get your head around but they are fairly consistent in their structure so once you get the hang of it it's not too bad. You invoke the manual pages with the following command:
`man <command to look up>`

>> long hand command line options begin with two dashes ( -- ) and short hand options begin with a single dash ( - )

<br>
<hr>

# 5- File Manipulation:
here you should know how to:

- Create a Directory:
by useing `mkdir [options] <Directory>` which is short for Make Directory..
also there is a few useful options available for **mkdir**:
* `-p` : which tells mkdir to make parent directories as needed (demonstration of what that actually means below)
* `-v` : which makes mkdir tell us what it is doing..

- Removing a Directory:
by useing `rmdir [options] <Directory>` also it supports `-v` & `-p` simillar to `mkdir`

>> *** a directory must be empty before it may be removed ***

so to remove the unempty files you should use `rm` command folowd with `-rf` then the dir.. :)

- Creating a Blank File:
by useing `touch [options] <filename>`
touch is actually a command we may use to modify the access and modification times on a file (normally not needed but sometimes when you're testing a system that relies on file access or modification times it can be useful)

>> Many things in Linux are not done directly but by knowing the behaviour of certain commands and aspects of the system and using them in creative ways to achieve the desired outcome..

- Copying a File or Directory:
by useing `cp [options] <source> <destination>`
also you should note that there is option that `cp` support, cuz default behaviour `cp` will only copy a file:
* `-r` :which stands for recursive, we may copy directories "eans that we want to look at a directory and all files and directories within it, and for subdirectories, go into them and do the same thing and keep doing this"

- Moving a File or Directory:
by useing `mv [options] <source> <destination>`
>> Renaming Files and Directories!
you can use the `mv` to rename the files like you just need to copy from the source to the new dir but with new file name...
its creative way :)

>> No undo!: The Linux command line does not have an undo feature. Perform destructive actions carefully :|

<br>
<hr>

# 6- Vi Text Editor:
Vi is a text editor that is most likely very different to any editor you have used before  (similar to Notepad) but like command line text editor..
Everything in Vi is done via the keyboard, There are two modes in Vi. Insert (or Input) mode and Edit mode..
use `vi <file>` to start vi text editor..
pressing `i` it will switch you to the insert mode, and press `Esc` will take you back to edit mode..
you can use:
- `ZZ` (Note: capitals) for Save and exit
- `:q!` for discard all changes, since the last save, and exit
- `:w` for save file but don't exit
- `:wq` for again, save and exit

. Other ways to view files:
there are two other commands which are a bit more convenient for that purpose:
* `cat` :which actually stands for concatenate like: `cat <file>`, and its always used with small files..
* `less` :witch is better suited for larger files, `less <file>`, allows you to move up and down within a file using the arrow keys. You may go forward a whole page using the SpaceBar or back a page by pressing b. When you are done you can press q for quit.

<br>
<hr>

# 7- Wildcards:
which is a set of building blocks that allow you to create a pattern defining a set of files or directories
* basic set of wildcards:
. `*` - represents zero or more characters
. `?` - represents a single character
. `[]` - represents a range of characters
actuly you can use it whenever you need in any command like:
`ls ??b*` :it will bring you all the files witch third letter will be 'b' letter..
or `ls *[0-9]*` :witch will bring any name had an digit in..

>> it is something like 'regex'..

<br>
<hr>

# 8- Permissions:
Linux permissions dictate 3 things you may do with a file:
. 'r' read - you may view the contents of the file.
. 'w' write - you may change the contents of the file.
. 'x' execute - you may execute or run the file if it is a program or script
and its all in Three persmissions and three groups of people:
. 'owner' - a single person who owns the file. (typically the person who created the file but ownership may be granted to some one else by certain users)
. 'group' - every file belongs to a single group
. 'others' - everyone else who is not in the group or the owner
* To view permissions for a file we use the long listing option for the command ls like: `ls -i [path]`
* To change permissions on a file or directory we use a command called chmod like: `chmod [permissions] [path]`
* Shorthand Premissions:
you can simply replace the letters with numbers debends on binary & 8 bits system (0,1 & 0-7) based on this colomn:
![cap](capture_cmd.PNG)
ex:
```
~$ chmod 240 frog.png
~$ ls -l frog.png
--w-r----- 1 harry users 2.7K Jan 4 07:32 frog.png
```
so now we know that 2 = 001 in binary
and 4 = 100 and 0 = 000
each groub of numbers in the premission is replaced with binary number so it will be like:
'-010100000'
>> as you know the first char is to define if this is file or dir(- or d or a) .. also as you know the premission cahars be like 'rwxrwxrwx'
the first for the "owner" and second for "group" and last for "others"..
so for '1 == on & 0 == off'
you will see the premission be like:
'- off on off on off off off off off'
and thats smae as: '--w-r-----'
as simpl as that.. :)
* Permissions for Directories:
The same series of permissions may be used for directories but they have a slightly different behaviour, use: `ls -ld` to view the dir premission..
. `r` - you have the ability to read the contents of the directory (ie do an ls)
. `w` - you have the ability to write into the directory (ie create files and directories)
. `x` - you have the ability to enter that directory (ie cd)
>> Normally, for optimal security, you should not give either the group or others write access to your home directory, but execute without read can come in handy sometimes. This allows people to get into your home directory but not allow them to see what is there..

<br>
<hr>

# 9- Filters:
in the context of the Linux command line, is a program that accepts textual data and then transforms it in a particular way, there is alot of filters like :
- head :
witch is a program that prints the first so many lines of it's input. By default it will print the first 10 lines but we may modify this with a command line argument, it look like: `head [-number of lines to print] [path]`
- tail :
witch is the opposite of head. Tail is a program that prints the last so many lines of it's input. By default it will print the last 10 lines but we may modify this with a command line argument, & looks like: `tail [-number of lines to print] [path]`
- sort :
Sort will sort it's input, nice and simple. By default it will sort alphabetically but there are many options available to modify the sorting mechanism, it looks like: `sort [-options] [path]`
- nl :
nl stands for number lines and it does just that, like: `nl [-options] [path]`
>> Note: spaces are normally used as separator characters on the command line
- wc :
it stands for word count and it does just that (as well as characters and lines). By default it will give a count of all 3 but using command line options we may limit it to just what we are after, it looks like: `wc [-options] [path]`
- cut :
it is a nice little program to use if your content is separated into fields (columns) and you only want certain fields, it looks like: `cut [-options] [path]`
>> Note: cut defaults to using the TAB character as a separator to identify fields, but you can specify it as you want..
- sed :
sed stands for Stream Editor and it effectively allows us to do a search and replace on our data. It is quite a powerful command but we will use it here in it's basic format: `sed <expression> [path]`
* the basic expression is of the following format:
`sed 's/search/replace/g' [path]`
- uniq :
uniq stands for unique and it's job is to remove duplicate lines from the data, it looks like: `uniq [options] [path]`
- tac :
The program tac is actually cat in reverse, Given data it will print the last line first, through to the first line..
`tac [path]`
- Tar :
Tar stands for Tape ARchive and is a popular means for combining and compressing several files into a single file. It was originally created for making backups on tape but is still commonly used today. Even though there are other options such as ZIP files for compression, tar remains popular as it is able to store filesystem information as well such as user and group permissions and dates..
it used like: 
```
~$ tar -zcvf mytar.tar.gz *
[this will create 'mytar.tar.gz' contain all the path contain..]
~$ tar -zxvf mytar.tar.gz
[and thats how it will excute to the same path also..]
```
<br>
<hr>

# 10- Grep and Regular Expressions:
* eGrep:
 it is a program which will search a given set of data and print every line which contains a given pattern. It is an extension of a program called grep. It's name is odd but based upon a command which did a similar function, in a text editor called ed. It has many command line options which modify it's behaviour so it's worth checking out it's man page, looks like:
`egrep [command line options] <pattern> [path]`
* regex:
 it is similar to the wildcards, They allow us to create a pattern. They are a bit more powerful however. Re's are typically used to identify and manipulate specific pieces of data, it is used all over the place..
. basic strategies:
1. check for typo's
2. always try to Re read the content here
3. Break your pattern down into individual components and test each of these individually
4. Examine your output
* the basic bulding blocks:
![cap](capture_cmd2.PNG)

<br>
<hr>

# 11- Piping and Redirection:
which means we may connect the three streams:
1. 'STDIN (0)' - Standard input (data fed into the program)
2. 'STDOUT (1)' - Standard output (data printed by the program, defaults to the terminal)
3. 'STDERR (2)' - Standard error (for error messages, also defaults to the terminal)
  between programs and files to direct data in interesting and useful ways..
* Normally, we will get our output on the screen, which is convenient most of the time, but sometimes we may wish to save it into a file to keep as a record, feed into another system, or send to someone else. The greater than operator ( > ) indicates to the command line that we wish the programs output (or whatever it sends to STDOUT) to be saved in a file instead of printed to the screen ex:
```
~$ ls
barry.txt bob example.png firstfile foo1 video.mpeg
~$ ls > myoutput
~$ ls
barry.txt bob example.png firstfile foo1 myoutput video.mpeg
```
>> When piping and redirecting, the actual data will always be the same, but the formatting of that data may be slightly different to what is normally printed to the screen
* Saving to an Existing File:
If we redirect to a file which does not exist, it will be created automatically for us. If we save into a file which already exists, however, then it's contents will be cleared, then the new output saved to it.
  by useing ( >> ) we can append the new data to the file..
>> Note: If we use the less than operator ( < ) then we can send data the other way. We will read data from the file and feed it into the program via it's STDIN stream..
* STDERR:
STDERR is stream number 2 and we may use these numbers to identify the streams. If we place a number before the > operator then it will redirect that stream (if we don't use a number, like we have been doing so far, then it defaults to stream 1)...
ex of STDERR:
![cap](capture_cmd3.PNG)
>> it also could be like `ls -l video.mpg blah.foo > myoutput 2>&1` so it will save the output and the errors to the same file..
* Piping:
it is the mechanism for sending data from one program to another, it use the operator (|), and what it dose do is feed the output from the program on the left as input to the program on the right..

<br>
<hr>

# 12- Process Management:
like most modern OS's many processes can be running at the same time in linux, If we would like to get a snapshot of what is currently happening on the system we may use a program called top. `top` :it will give you a realtime view of the system and only show the number of processes which will fit on the screen..
* Another program to look at processes is called ps which stands for processes `ps` , it will show you just the processes running in your current terminal..
>> If we add the argument aux then it will show a complete system view which is a bit more helpful!
* Killing a Crashed Process:
you will need first to identify the proccess id..
```
~$ ps aux | grep 'firefox'
ryan 6978 8.8 23.5 2344096 945452 ? Sl 08:03 49:53 /usr/lib64/firefox/firefox
```
thwn you can use kill program like:
`kill [signal] <PID>`
```
~$ kill -9 6978
```
Done..! :)
* Foreground and Background Jobs:
use `jobs` :
Display a list of current jobs running in the background
or use `fg` :to Move a background process into the foreground!
or you can simply use `ctrl + z` :to Pause the current foreground process and move it into the background..

<br>
<hr>

# 13- Scripting:
witch is computing terms is similar to a script in theatrical terms. It is a document stating what to say and do. Here, instead of the script being read and acted upon by a person, it is read and acted upon (or executed) by the computer..
>> Anything you can run on the command line you may place into a script and they will behave exactly the same
* The Shebang:
The very first line of a script should tell the system which interpreter should be used on this file. It is important that this is the very first line of the script. It is also important that there are no spaces. The first two characters #! (the shebang) tell the system that directly after it will be a path to the interpreter to be used. If we don't know where our interpreter is located then we may use a program called which to find out:
`which <program>`
* The Name:
Linux is an extensionless system. That means we may call our script whatever we like and it will not affect it's running in any way. While it is typical to put a .sh extension on our scripts, this is purely for convenience and is not required
* Comments:
use `#` in start of any line to make it comment
* Why the ./ ? :
Linux is set up the way it is, largely for logical reasons. This peculiarity actually makes the system a bit safer for us. First a bit of background knowledge. When we type a command on the command line, the system runs through a preset series of directories, looking for the program we specified. We may find out these directories by looking at a particular variable 'PATH', 
The system will look in the first directory and if it finds the program it will run it, if not it will check the second directory and so on. Directories are separated by a colon ( : ), The system will not look in any directories apart from these, it won't even look in your current directory. We can override this behaviour however by supplying a path. When we do so the system effectively says "Ah, you've told me where to look to find the script so I'll ignore the PATH and go straight to the location you've specified instead." You'll remember from section 2 (Basic Navigation) that a full stop ( . ) represents our current directory, so when we say ./myscript.sh we are actually tellling the system to look in our current directory to find the script. We could have used an absolute path as well ( /home/ryan/linuxtutorialwork/myscript.sh ) and it would have worked exactly the same, or a relative path if we are not currently in the same directory as the script ( ../linuxtutorialwork/myscript.sh ), If it were possible to run scripts in your current directory without this mechanism then it would be easy, for instance, for someone to create a malicious script in a particular directory and name it ls or something similar. People would inadventently run it if they wanted to see what was in that directory!!((thats realy good point..!!))
* Permissions:
A script must have the execute permission before we may run it (even if we are the owner of the file). For safety reasons, you don't have execute permission by default so you have to add it. A good command to run to ensure your script is set up right is `chmod 755 <script>`

- Variables:
A variable is a container for a simple piece of data
* When we set a variable, we specify it's name, followed directly by an equals sign ( = ) followed directly by the value. (So, no spaces on either side of the = sign.)
* When we refer to a variable, we must place a dollar sign ( $ ) before the variable name, ex:
```
~$ cat variableexample.sh
#!/bin/bash
# A simple demonstration of variables
# Ryan 15/8/2020
 
name='Ryan'
echo Hello $name
~$
~$ ./variableexample.sh
Hello Ryan
```
* Command line arguments and More:
When we run a script, there are several variables that get set automatically for us. Here are some of them:
1. '$0' - The name of the script
2. '$1 - $9' - Any command line arguments given to the script. $1 is the first argument, $2 the second and so on...
3. '$#' - How many command line arguments were given to the script
4. '$*' - All of the command line arguments
>> `echo` == print
* Back ticks:
it used to save the output of a command to a variable and the mechanism we use for that is the backtick ( ` )..

- If Statements:
* we use `fi` To indicate the end of an if statement we have a single line which has fi (if backwards) on it
* The command `read` is asking the user to input..
 >> If statements actually make use of a command called test
```
if [ ] then else fi
Perform basic conditional logic
```

<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)
