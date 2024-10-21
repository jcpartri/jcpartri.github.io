# Navigating Your Computer

&#x2637; [Table of Contents](./../toc.md)

> **Note for Windows Users:** If you successfully installed WSL in the last lesson, then just make sure it is the default integrated terminal you are using in VS Code and you will proceed fine from here.
>
> If you DID NOT have success installing WSL, then some features in this lesson will not work. That is ok. It is not vital that it does. Do what you can and leave the rest alone. Smile! you are doing ok!
>
> For those without WSL: The Windows file system uses backslashes `\` to indicated separations in directories.

## Lesson Outline

[pwd](#pwd) | [ls](#ls) | [ls -a](#ls--a) | [The Wildcard](#the-wildcard-) | [Clearing the Terminal](#clearing-the-terminal-screen) | [Clibming and Diving](#climbing-and-diving) |  [Changing Directories](#changing-directories) | [Autocomplete](#autocomplete) | [Going Up One Level](#going-up-one-level) | [Absolute Path and Root](#absolute-path-and-root) | [The Current Directory](#the-current-directory) | [Relative Paths](#relative-paths) | [Terminal Magic](#terminal-magic) | [Beyond Python](#-beyond-python) | [Challenge](#challenge) | [Summary](#summary)

## Introduction

> &#128214; John 17:20 - I do not ask for these only, but also for those who will believe in Me through their word.

Have you ever wondered how the gospel came to you? In this lesson we are going to learn how to navigate through a computer's file system, and then we are going to take some ideas that we learn from this lesson and use it to discuss this very question. _"How did the gospel find me?"_

---

Your computer is made up of a **file system**. A file system is a set of directories (folders) and files on the computer that are interconnected and related to each other in a 'tree' like shape. All files and directories in a file system are connected ultimately to the same root.  

A file system has a **root**. In Windows, the root is denoted by the symbol `C:\\` (also known at the C drive.) 

On MacOS or Linux systems, the root is denoted by a single forward slash. `/`. Here is a simplfied illustration of a file system.

The _root_ of a file system is the highest level directory. It is the directory that is not contained by any other directory. The _root_ is the directory that contains all other directories and files.

![A File System](../images/a%20simple%20filesystem.png)

---

**Open VS Code and then open the integrated terminal in VS Code.** If you do not remember how to do this, return to the previous lesson for directions.

---

## `pwd`

`pwd` stands for _print working directory_. Think of a directory as a folder on your computer. The two words **directory** and **folder** are synonyms. `pwd` tells you where you are currently located on your system. The folder you are located in is called your **working directory**.

When you use `pwd` you get a **_path_** as output.

```terminal
$ pwd
C:\\Users\username\Documents\projects\books\pwawv
```

The example above means that I am currently located in the `pwawv` folder. `pwawv` is the last folder name in the path above and therefore it is the folder I am currently located in. It is my _working directory_.

> **Imporant Note:** On Windows ![win logo](../images/win11_logo.png), you use a backslash `\` to indicated a new folder or directory. 
>
> If Windows Users have WSL installed in their system, then they can use the forward slash `/` as the separator.
> 
> On MacOS ![apple logo](../images/apple_logo.png) and Linux ![linux logo](../images/my_tux.gif), you use a forward slash `/`.
>
> Knowing the difference now will help you as you progress through this text.

## `ls`

`ls` stands for _list_. It lists all the files and folders that are located inside of your current working directory.

```console
$ ls
Mode                 LastWriteTime         Length Name   
----                 -------------         ------ ----   
d-r--          12/10/2023  3:44 PM                3D Objects
d-r--          12/10/2023  3:44 PM                Contacts
d-r--           3/25/2024 10:41 AM                Desktop
d-r--            6/5/2024  4:43 PM                Documents
d-r--          12/12/2022  4:09 PM                Downloads
d-r--          12/10/2023  3:44 PM                Favorites
```

What you are seeing in the example above is the `ls` command used on a Windows ![win logo](../images/win11_logo.png) system.

MacOS ![apple logo](../images/apple_logo.png) and Linux ![linux logo](../images/my_tux.gif) organize their files and folders a bit differently._ Here is what I get when I use the `ls` command on my Mac.

```console
$ ls
Applications    Users           cores           home            sbin            var
Library         Volumes         dev             opt             tmp
System          bin             etc             private         usr
```

### `ls -a`

Sometimes a command in the terminal comes with an option or two. We can show hidden files by using the `-a` option. `ls -a` will show all files and folders along with all hidden files. Hidden files begin with a period.

```console
ls -a
Mode                 LastWriteTime         Length Name   
----                 -------------         ------ ---- 
d----          12/18/2023 11:17 AM                .fly   
d----           8/22/2022  3:56 PM                .idlerc
d----           9/25/2023  2:56 PM                .MakeMKV
d----          12/15/2023  8:24 PM                .ssh
d----           8/28/2023  3:40 PM                .vscode
d-r--          12/10/2023  3:44 PM                3D Objects
d-r--          12/10/2023  3:44 PM                Contacts
d-r--           3/25/2024 10:41 AM                Desktop
d-r--            6/5/2024  4:43 PM                Documents
d-r--          12/12/2022  4:09 PM                Downloads
d-r--          12/10/2023  3:44 PM                Favorites
```

_If you create your own text file, begin the filename with a period. It will become a hidden file that you cannot see unless you use the `ls -a` command. It is possible to show all hidden files on your computer by default, but that is left for you to research on your own._

### The Wildcard `*`

If you are looking for a specific file or folder you can use the `*` wildcard. Lets say I am looking for my `Documents` folder.

```console
ls D*
d-r--           3/25/2024 10:41 AM                Desktop
d-r--            6/5/2024  4:43 PM                Documents
d-r--          12/12/2022  4:09 PM                Downloads
```

> _Notice that it finds everything that begins with a `D` and then gives me all the file/folder options from that point._

> If you typed `ls *a*` this would find any files or folders that contains a lowercase 'a' in them.

### Clearing the Terminal Screen

In the terminal window if you want to clear the screen you can hit the `CTRL + L` combination on your keyboard. Go ahead and give it a try. In Windows you can also type `cls`. On MacOS or Linux you can also type `clear` and then hit the `Enter/Return` key.

![terminal logo](../images/terminal_icon.png)

> Note: `CTRL + L` unfortunately does not work in Windows Command Prompt. `cls` does however.

### Climbing and Diving

In the very next section we are going to look at the `cd` command. This is the primary command used when navigating your file system. 

We are going to use the phrases "climb" and "dive" to illustrate going upwards and downwards in the file system. Be prepared when we begin to use this terminology.

### Changing Directories.

Remember that the word `directory` is synonymous with the word `folder`. Let's say I type `pwd` to see where I am located on my system, and then type `ls` to see what is listed in that folder.

```console
$ pwd
C:\\Users\username\Documents\projects\books\pwawv
$ ls
Mode                 LastWriteTime         Length Name   
----                 -------------         ------ ---- 
d----          12/18/2023 11:17 AM                chp0 
d----          12/18/2023 11:17 AM                chp1  
d----           8/22/2022  3:56 PM                chp2
d----           9/25/2023  2:56 PM                chp3
```

**Question:** How do I navigate from where I am into the chp1 folder? By using the `cd` command. `cd` stands for _change directory_.

```console
$ cd chp1
$ pwd
C:\\Users\username\Documents\projects\books\pwawv\chp1
$
```

At first it looked like nothing happened, but when I typed in the `pwd` command I can now see that I am in the `chp1` folder. We "dove downwards" from the `pwawv` folder into the `chp1` folder.

`cd` is the primary command we need in order to navigate our file system.

### Autocomplete

A really nice feature is _auto complete_ in the terminal window. Let's say I am in a folder named `temp` and inside this folder is another folder named: `long_folder_name_because_I_like_difficult_things`.

```console
$ pwd
/Users/username/Documents/temp
$ ls
folder_1            folder_2
long_folder_name_because_I_like_difficult_things
$ cd lon
```

You can type `cd lon` and then hit the `TAB` key on your keyboard. The terminal will auto complete it for you!

```console
$ cd long_folder_name_because_I_like_difficult_things
```

Coll huh!!!

### Going Up One Level

So how do I go back "upwards" again back to the `pwawv` folder which is where I was originally? If I use two period `..` with the `cd` command, this is the same as saying go back/up one level.

```console
$ pwd
C:\\Users\username\Documents\projects\books\pwawv\chp1
$ cd ..
$ pwd
C:\\Users\username\Documents\projects\books\pwawv
$
```

In the example above we "climbed upwards" from the `chp1` folder back into the `pwawv` folder.

### Absolute Path and Root

It is important at this point of the lesson to state that any given path that traverses back to the **root** of the system is called an **absolute path**. On a Windows machine, the root of the system is known as the `C:\\` drive. On MacOS and Linux however, the root is a single forward slash `/`

Here is an example of an absolute path on MacOS

```console
$ pwd
/Users/username/Documents/work/office
$
```

![illustration of root on mac or linux](../images/illustration%20of%20root%20on%20mac%20and%20linux.png)

The very first `/` is the root of the system. Every `/` that follows just denotes a folder/directory beneath the one before it. Here is a tree/path diagram illustrating the path above.

![folder heirarchy](../images/chp0_folder_heirarchy.png)

### The Current Directory

Yes, there is even a symbol for the current directory you are in. It is a period. `.` Yup, a period. Therefore if you see the following path...

`./office/other/myforms`

This means "Begin in the current directory, then proceed to the `office` folder, then to the `other` folder, and finally to the `myforms` folder."

### Relative Paths

Unlike absolute paths, **relative paths** are connected to where YOU are currently located on the system. To put it another way, they are _relative_ to your location, not to the root.  Let's say that I am in the `office` folder.

```console
$ pwd
/Users/username/Documents/work/office
$ cd ../home/business
$ pwd
/Users/username/Documents/work/home/business
```

`../home/business` is a relative path. This means, "Go up one level from the `office` folder, then dive down into the `home` folder and then dive down one more time into the `business` folder. Below is a diagram.

![folder heirarchy 2](../images/chp0_folder_heirarchy_2.png)

## Terminal Magic

> **Note for Windows Users:** If you did not have success installing WSL on your system, then the `touch` command given in this lesson will not work. Neither will the iterative mkdir command: `mkdir file{1..9}.txt`:frowning:
>
> You may be able to replace the `touch` command with the following command: `echo $null >> `
>
> **Note for Windows Users:** If you DID have success installing WSL, then make sure it is the primary terminal in the integrated terminal environment in your VS Code editor.

Are you ready to feel like a 99th level programming guru? Try this...

**Step 1:** Open you terminal window in VS Code.

**Step 2:** Navigate to your `Documents` folder. Usually found in `C:\\Users\username\Documents` on Windows and `/Users/username/home/Documents` on MacOS.

**Step 3:** type `touch temp.txt` then hit `Enter/Return`

**Step 4:** Now type: `ls`

You just created an empty text file! Do you see it in the list?

> **touch**: The `touch` command actually just updates the timestamps on files and folders. If however, the file does not exist it creates the file and then adds the timestamp. Timestamps allow you to see when a file was last modified. This gives `touch` the illusion that it was made to create empty files. 

You can also create your own directories/folders with the `mkdir` command.

**Step 5:** Type `mkdir temp_folder`

**Step 6:** Now type: `ls`

Now both `temp.txt` and `temp_folder` should appear in the listing.

> **mkdir**: The `mkdir` command is short for _make directory_. It does exactly what the command suggests. It makes a directory. Remember, that directory and folder are synonymous terms.

Now let's do something really cool! Use the `cd` command to navigate into the `temp_folder` you just created.

**Step 7:** Type `mkdir folder{1..9}` and hit `Enter/Return`.

**Step 8:** Now type: `ls`

> **iterative processes**: The command `mkdir folder{1..9}` makes nine folders using an iterative process. Iterative means to repeat something. Therefore, the command makes a folder1, folder2, ... all the way up to folder9.

## Challenge

If you want to learn how to delete files and folders on your system, then we recommend you learn the highly useful, yet dangerious, `rm` command. `rm` must be used with extreme caution however.

Here is a link to an article from **howtogeek.com** on using the `rm` command safely: https://www.howtogeek.com/858815/linux-rm-command/

> **Warning:** Do not damage your system! If you don't need to delete something, then don't use the `rm` command.

## Summary

So, lets ask the question: _"How did the gospel find me?"_. Remember the verse given at the beginning of this lesson? John 17:20. "I do not ask for these only, but also for those who will believe in Me through their word."

There is no website on earth that tracks your ancestry that could handle the sheer complexity of how the gospel came from the apostles, through the centuries, down to your doorstep and into your heart and life. [^1] Since this gospel has followed a path, we can attempt to make something like a tree diagram for it.
 
![How Did the Gospel Find Me?](../images/howdidthegospelfindme.png)


The fact that it did come to you is no mistake. It was God ordained. When Jesus prays for _those who come to believe through their (the apostles) word._ He is praying for you.

---

In this lesson we learned how to do the following.

* Use the `pwd` command. `pwd` stands for print working directory.
* Use the `ls` command. `ls` stands for list.
* Use the `-a` option with the `ls` command. `-a` shows all files in the current working directory. Even the hidden ones.
* Use the wildcard `*`. The wildcard represents characters or digits or punctuation symbols when performing a search for an file or folder using `ls`.
* How to clear the terminal with the `CTRL + L` key combination.
* How to clear the terminal with either the `cls` or `clear` commands. Know which operating systems require either `cls` or `clear`.
* Using the `cd` command to change directories. This is a primary command that we use to navigate our system.
* The meaning and difference between and absolute and relative paths.
* The symbol for the current working directory is `.`
* Autocomplete feature in the terminal.
* Using the `..` prefix to rise up one level in the directory heirarchy using the `cd` command.
* `root`. Remember that root on Windows is `C:\\`. On MacOS and Linux the root is `/`.
* Creating timestamps and new files with the `touch` command.
* Creating new folders with the `mkdir` command.
* Iterative processes using `{1..9}` as an example.

---

**Projected Lesson Read Time: 15 minutes**

&#8678; Previous Lesson: [The Terminal and CLI's](./005_the_terminal_and_clis.md)

&#8680; Next Lesson: [Compressing Files](./007_compressing_files.md)

[^1]: "_How Jesus Thinks About Us_" by Dr. Sinclair Ferguson. Resource: https://www.youtube.com/watch?v=vUJnOYGPzHU