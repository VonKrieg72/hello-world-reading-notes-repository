# The Coder's Computer

## Text Editor

A text editor is software that you can either download onto your computer, or have access to online. Text editors enable you to write, organize, and manage text, in particular, the text that you write to build up a website. Some important features that you would want to make sure a text editor has are

***-Code completion***

***-Syntax highlighting*** 

***-A nice variety of themes***

***-The ability to choose from a healthy selection of extensions available when you need them***

Code completion provides you with possible options or suggestions when you start typing, which minimizes the possibility for you to make typos or errors in your code. Syntax highlighting takes what you type and changes it to different colors to make them more noticeable, which makes it more easier for you to find typos and errors. For example, attributes, elements, and copy will all be different colors. Themes will enable you to change the color of the background in your text editor. Usually developers will choose darker background with bright letters, to reduce eye strain and fatigue. Extensions give you the ability to add on more features to yor text editor, like an upgrade. 

It's important to point out that all of your computers will come a text editor pre-installed. For example, Mac Os will come with a pre-installed text editor called "Text Edit", Windows Os will come with "Notepad", and Linux Os will come with different text editors installed, depending on your particular distribution. However, the text editors that come pre-installed on your computer won't come with the features mentioned earlier, such as code completion, syntax highlighting, a nice variety of themes, and the ability to choose from a healthy selection of extensions available when you need them. This is important to point out, because with no code completion, it will be easier for you to make typos or errors, which you'll be responsible to edit on your own. 

Just to name a few third party text editors that you can download onto your computer, you can choose

***-Notepad (for Windows Os only)***

***-BB Edit, which has incorporated the former Text Wrangler into it (for Mac Os only)***

***-Visual Studio, which was made by Microsoft (available for Windows, Mac, and Linux)***

***-Atom, which is from Github (available for Windows, Mac, and Linux)***

***-Brackets, which is from Adobe (available for Windows, Mac, and Linux)***

You also have the option to use an Integrated Development Environment (IDE) instead of a regular text editor. IDEs have multiple different types of software in them. An IDE is a text editor, file manager, compiler, and a debugger all in one. 

## The Command Line

A command Line, which is sometimes called a terminal is a text based interface to the system, which enables you to enter commands by typing them on the keyboard, in which feedback or a message will be given to you as a reply text. The command line in most cases will present you with a prompt **(user@bash)**, and as you type it will show up after the prompt **(ls)**. in most cases you'll be issuing the command. Then command line arguments will pop up **(-l/home/ryan)**. All of these commands and command line arguments will be seperated by a space. 

**user@bash: ls -l/home/ryan**

After you type this, the system will display output from running the command, and then another prompt will be presented again **(user@bash)**. This is how you know the command has run, and the terminal is ready for you to enter anoter command. If no prompt is presented, then your command is probabaly still running. 

## Basic Navigation

The **pwd** command, which stands for *print working directory,* tells you where you are currently, and what your present working directory is. This can be useful, if you're moving around alot while entering code, and you need to know where you are or where you left off. The **ls** command, which stands for *list* tells you what is there as oppossed to the pwd command, which tells you where you are. When you enter the **-l** command, it's saying that you want a long list. The first character **(-)** indicates a normal file, or a directory. The **/etc** command tells you to list that directories contents.  

A path means to get a particular file or directory on the system, and whenever you enter a file or directory on the command line it is a path. There are two types of paths: **absoulte paths** and **relative paths.** Absolute paths specify a location (file or directory) in relation to the root directory, and they always begin with a forward slash **(/).** Relative paths specify a location (file or directory) in relation to where we currently are in the system. These will not begin with the forward slash. You can refer to a location in a variety of different ways, and you can use any method you like to refer to a location. Whenever you refer to a file or directory on the command line, you're referring to a path, which can be constructed using any of these elements. The **cd** command enables you to move around the system. If the **cd** command is run without any arguments, it will take you back to your home directory. 

## More About Files

In the Linux Os everything is actually a file. This includes things such as text, a directory, your keyboard (system reads from), and your monitor (system writes to). A file extension is normally a set of 2-4 characters, after a full stop at the end of a file, which tells you what type of file it is. Some common file extensions include....

-file.exe - an executable file or program

-file.txt - a plain text file

-file.png - file.gif, file.jpg-an image

In Windows Os, the system uses the extensions to determine what type of file it is. In the Linux Os, the system looks inside the file to determine what type of file it is, while ignoring the extension. Unlike Windows Os, which is not case sensative, the Linux Os is case sensative. So, it's possible to have two or more files or directories with the same name, but letters with a different case. Case sensativity in Linux Os also applies to command line options as well. For example, the command **ls** is different from another command **lS,** in which the S is capital in one and lower case in the other. Keep this in mind when entering commands in Linux, or the output by the system will be something totally different from what you're expecting.

It's important to remember on the command line that spaces seperate items. In order to go around this, you can either use single or double quotation marks. For example.....

-user@bash: cd 'Holiday Photos'

-user@bash: cd "Holiday Photos"

or you can use a backlash, which is known as an escape character. For example.....

-user@bash: cd Holiday\ Photos

The backlash nullifies the special meaning of the next character.

The Linux Os also has hidden files in it. Any file that begins with a dot **(.)** is a hidden file. You don't need any special commands to make files hidden, just put a dot **(.)** in the beginning when you name it. If you wish to make a hidden file unhidden, just re-name it by removing the dot before the name. If you wish to list the hidden files in the command line, you have to modify the **ls** command, by including the command line option **-a.** For example.....

-user@bash: ls Documents

-FILE1.txt.File1.txt file1.TXT

-.....

-user@bash: ls -a Documents 


[<== Back](README.md)
