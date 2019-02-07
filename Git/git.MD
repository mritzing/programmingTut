# Working With Git
This tutorial will assume you know how to navigate in your system's terminal window. 
### What isGit
Git is the most widely used version control system.  Version control systems allow you to neatly store and track changes in your files.  Git is often used in programming teams to enable non-linear development, or a development workflow where different people are working together on the different parts of the same project.  
There is a lot to learn in git but for now we will just deal with working in your own repository.


### Get Git
First you will need to download and install git which you can do from here, https://git-scm.com/.  When you are installing it check the box that says add to PATH.  Once git is installed make sure it is in your path by opening a terminal and typing 
```
git --version
```
If that command doesn't return an error message move on to the configuration. 
Windows Specific: 
If it does return a message saying something along the lines of git command not found you will need to add it to your path, the path is an enviroment variable which stores the location of executable programs on your computer allowing you to access them within the terminal.  First find where git was downloaded to in my case it was, "C:\Program Files\Git\bin", you need to link to the bin directory because that is where the git executable is located, copy the path to git's bin directory.  Next, in the start menu if you start typing "enviroment variables" you should see "Edit the system enviroment variables", which will take you to the "Advanced" of the Systems Properties panel.  Click on the "Enviroment Variables" button in the bottom right which will open a new window.  In the bottom half of that window, the System variables section, scroll until you find the "Path" variable and then double click it so you can edit it.  In the Edit enviroment variables window click the "New" button in the top right and then paste in the path to git's bin folder that we found before.  After you do this click ok on both windows to exit and save your changes.  Then open a new terminal window and run the command above and git should now work. 

### Using Git
Diagram ! 
In your terminal make a directory called "git_tutorial" and navigate into it (mkdir then cd).  Then create a file in the directory, you can do this with which will create a file called "HelloWorld.txt" with the contents "HelloWorld"
``` bash 
echo "Hello World" >> HelloWorld.txt
```

First we need to initialize the directory we are in as a git repository, do this with the command "git init".
Next we need to add the files that are ready to be commited to the local repository.  To do this use the add command, you can add a file by its name "git add HelloWorld.txt" or add all files with the "*", you can also choose to add just certain files, for example if you only wanted to include the python files in your directory you would run "git add *.py"
``` bash 
git add *
```
You can see the files that are ready to be commited if you run "git status", this command also will show files that have not been added to the current commit.  You should see the file that you just added as a file staged for commit.  To commit the files to the local repository use the "git commit" command followed by -m and a message in quotes.  The message should generally be descriptive of what files are being added/changed.  
``` bash
git commit -m "First Commit"
```



### Getting Files Onto a Remote Repository
Git is the tool we will be using to store our files but we still need a place to put them so we will use github.com, there are many alternatives but github is the most popular.  Once you created and account and logged in find the button to create a new repository, a green button in the repository section of the site.  

### Ignoring Files



#### Vocabulary: 
* Version Control System: Manages changes of files
* Repository: A location where your files are stored and managed. 

#### Commands:
* git add: stages files ready to be commited to local repository
* git commit: adds ready files to local repository , use -m option to add a message
* git push: puts files in local repository onto remote repository
* git log: prints commit history
* git status: prints which files are currently staged for commit
* git clone: Creates a copy or clone of target repository
    * for example to clone this (https://github.com/mritzing/exifProc) this repository, you would run "git clone https://github.com/mritzing/exifProc.git", the link comes from the green "Clone or download" button on the repository page
    *