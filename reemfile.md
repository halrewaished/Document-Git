# **GIT**
#### with files :


1 -  In working tree ' our folder ' we write **git init** command to create **.git** 
file.
Which contains all of the necessary Git metadata for the new repository. This metadata 
includes subdirectories for objects, refs, and template files. A** HEAD** file is also 
created which points to the currently checked out commit.

           $ git init


2 - Each file in your working directory can be in one of two states: tracked or 
untracked. Tracked files are files that were in the last snapshot, as well as any newly 
staged files; they can be unmodified, modified, or staged. In short, tracked files are 
files that Git knows about.
Any files in your working directory that were not in your last snapshot and are not in 
your staging area.
The main tool you use to determine which files are in which state is the **git status** 
command.

        $ git status

In order to begin tracking a new file, you use the **git add** command.

	$ git add <file name> or . 

3 -  Now that your staging area is set up the way you want it, you can commit your 
changes. Remember that anything that is still unstaged — any files you have created or 
modified that you haven’t run git add on since you edited them — won’t go into this 
commit.

        $ git commit -m "type your commit message" 
