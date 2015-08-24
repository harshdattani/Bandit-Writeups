Bandit Writeups
===================

Writeups of how I solved **Bandit** questions, might be usefull to those who are stucked in any level.
I have not posted **Keys** to next level. Just steps to complete the level! :P If you have any trouble solving the levels, create an issue in this Repo, will try to resolve it :)

> **Note:** Every Bandit Level provides list of commands to be used and a prerequisites to solve perticular challenge. 

----------

Level 0
-------------
> **Level Goal:** 
The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH to log into that level and continue the game.

 1. An easy level, just login using ssh in **bandit.labs.overthewire.org** using username: **bandit0** and the password **bandit0**.
 2. Use our favourite **ls** to view files/folders and **cat** to read contents of **readme**.
 
    `cat readme`
 3. This file contains the password to next Bandit01 level.

Level 1
-------------
> **Level Goal:** 
The password for the next level is stored in a file called - located in the home directory.

 1. Login to **bandit1** via ssh and password.
 2. Use **ls** and notice a file named "**-**". Open it and password will be yours! :P
   `cat ./-`

Level 2
-------------

 > **Level Goal:** 
The password for the next level is stored in a file called spaces in this filename located in the home directory.

 1. Login to **bandit2** via ssh and password.
 2. Use **ls** and notice a file named "**spaces in this filename**".
 3. Open it using **cat** and password will be yours!
 
   `cat spaces\ in\ this\ filename` 
 >**Hint:** Use **Tab** key instead of typing whole file name.

Level 3
-------------

 > **Level Goal:** 
The password for the next level is stored in a hidden file in the inhere directory.

 1. Login to **bandit3** via ssh and password.
 2. Navigate to **inhere** directory using **cd** command.
 3. Use **ls -a** to view all files, including hidden files and folders.
 4. Open the hidden file using **cat** and passwordis yours.

 `cat .hidden`
 >**Tip:** All hidden file names start with a **.** in Linux.


Level 4
-------------

 > **Level Goal:** 
The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

 1. Login to **bandit4** via ssh and password.
 2. Navigate to **inhere** directory.
 2. Use **file ./*** command to find Human Readable i.e. an ASCII Text File and open that file using **cat**.

 `file ./*`

Level 5
-------------

 > **Level Goal:** 
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties: - human-readable - 1033 bytes in size - not executable.

 1. Login to **bandit5** via ssh and password.
 2. Navigate to **inhere** directory.
 2. Use **find** command to find Human Readable file with 1033 bytes size.

 `find ./* -size 1033c`
