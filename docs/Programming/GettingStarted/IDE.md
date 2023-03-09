# IDEs, Editors, and Terminal

## How development tools and the command line work
- The command line is a program that allows you to interact with the computer. It is a text based interface that allows you to type commands to the computer. It is very similar to how you interact with the computer using a GUI (Graphical User Interface). The only difference is that instead of using a mouse and clicking on buttons, you type commands to the computer.
- The command line is very powerful, and it is the most efficient way to interact with the computer. It is also the most efficient way to develop software aswell.
- This is why we have such a big emphasis on using Linux and its kernel, and why we recommend you use the command line to develop software for SCRobotics.
- Whilst any development tool will work, the next section we will explain why we recommend you use a text editor or the command line to develop software for SCRobotics instead of an IDE.

-----------------------------------------

## IDEs vs Editors
- Most tools you used before *(whether it is through academia or Youtube tutorials)* like Esclipse, Visual Studio, CLion, etc. are IDEs (Integrated Development Environment). They work by providing a GUI (Graphical User Interface) to interact with the computer, and they are usually used to develop software. 
- In reality, they are just a bunch of programs that are bundled together to make it easier for the user to use them. For example, Eclipse is a Java IDE, and it is made up of a bunch of Java programs that are bundled together to make it easier for the user to use them. The same goes for Visual Studio, CLion, etc... 
- You can achieve the same thing by using the command line or a regular text editor *(Notepad works just as well if not faster if you know what you're doing)*, it is often much easier and efficient to use than an IDE.
- IDEs are great for beginners because they provide a GUI to interact with the computer, and they are usually very easy to use. However, they are not as efficient as using the command line or a regular text editor.
- Which is why we recommend you use a text editor or the command line to develop software for SCRobotics.
- Again, use whatever you are comfortable with, as long if you know what you're doing. Same idea applies, all tools work the same way.
- These are tools we recommend you using (in order of preference):
    - [Visual Studio Code](https://code.visualstudio.com/) (VSCode)
    - [Sublime Text](https://www.sublimetext.com/)
    - [Nano](https://www.nano-editor.org/)
    - [Vim](https://www.vim.org/)

-----------------------------------------

## Terminal
- The terminal is a program that allows you to interact with the computer. It is a text based interface that allows you to type commands to the computer. It is very similar to how you interact with the computer using a GUI (Graphical User Interface). The only difference is that instead of using a mouse and clicking on buttons, you type commands to the computer.
- Common commands you should know or be familiar with:
    + `cd` - Change directory
    + `ls` - List files in the current directory
        + Example: If my terminal looks like this:
        ```bash
        jasper@wlux: /home/jasper$
        ```
        + This means I am in the `/home/jasper/` directory or "Home from the user Jasper". If I type `ls` into the terminal, it will list all the files in the `/home/jasper/` directory.
        ```bash
        jasper@wlux: /home/jasper/$ ls
        Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
        ```
        + I could then now type `cd Desktop` to change my directory to the `/home/jasper/Desktop/` directory.
        ```bash
        jasper@wlux: /home/jasper/$ cd Desktop
        jasper@wlux: /home/jasper/Desktop$
        ```
        + I could then type `ls` again to list all the files in the `/home/jasper/Desktop/` directory.
        ```bash
        jasper@wlux: /home/jasper/Desktop/$ ls
        ```
        + If I wanted to go back to the `/home/jasper/` directory, I could type `cd ..` to go back to the parent directory.
        ```bash
        jasper@wlux: /home/jasper/Desktop/$ cd ..
        jasper@wlux: /home/jasper/$
        ```
    + `mkdir` - Make a directory
    + `rm` - Remove a file
    + `rmdir` - Remove a directory
    + `mv` - Move a file or directory
    + `cp` - Copy a file or directory
    + `cat` - Print the contents of a file
    + `touch` - Create a file
        + Example: If I wanted to create a Python file called `main.py`, I could type `touch main.py` into the terminal.
        + But first, let's create a directory called `dev/` to store all our source code in.
        ```bash
        jasper@wlux: /home/jasper/$ mkdir dev
        jasper@wlux: /home/jasper/$ cd dev
        jasper@wlux: /home/jasper/dev/$ touch main.py
        jasper@wlux: /home/jasper/dev/$ ls
        main.py
        ```
    + `sudo` - Run a command as the superuser
        + Example: If I wanted to install a program, I would need to use `sudo` to run the command as the superuser.
        ```bash
        jasper@wlux: /home/jasper/dev/$ sudo apt install python3
        ```
    + `sudo apt-get update` - Update the package list
    + `sudo apt-get upgrade` - Upgrade all installed packages
        + Usually you would run these two commands before installing any program.
        + This is because the package list and installed packages may be outdated.
        + If you don't update the package list and installed packages, you may not be able to install the program you want.
        ```bash
        jasper@wlux: /home/jasper/dev/$ sudo apt-get update && sudo apt-get upgrade
        ```
        + Note: `&&` is a command that allows you to run multiple commands in one line. You can also use `;` to do the same thing.
    + `sudo apt-get install` - Install a program
        + Example: If I wanted to install Python 3, I would type `sudo apt-get install python3` into the terminal.
        ```bash
        jasper@wlux: /home/jasper/dev/$ sudo apt-get install python3
        ```
    + `sudo apt-get remove` - Remove a program
        + Example: If I wanted to remove Python 3, I would type `sudo apt-get remove python3` into the terminal. **(ALSO PLEASE DON'T UNINSTALL PYTHON3, DON'T ACTUALLY RUN THIS LMAO)**
        ```bash
        jasper@wlux: /home/jasper/dev/$ sudo apt-get remove python3
        ```
    + `sudo apt-get autoremove` - Remove all unused packages
        + Example: If I wanted to remove all unused packages, I would type `sudo apt-get autoremove` into the terminal.
        ```bash
        jasper@wlux: /home/jasper/dev/$ sudo apt-get autoremove
        ```
- You can find more commands [here](https://ss64.com/bash/).