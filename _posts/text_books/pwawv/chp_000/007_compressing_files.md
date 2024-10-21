# Compressing Files

> **Note &#9888;** Make sure to try each of these code snippets below on your own. Don't just read. Do! You will learn more from typing the code and making mistakes along the way than you will from just reading.

&#x2637; [Table of Contents](./../toc.md)

## Lesson Outline

[Create An Empty Project](#create-an-empty-project) | [View the Contents](#view-the-contents) | [Compress in Win/Lin](#compress-in-windows--linux) | [Compress in MacOS](#compress-in-macos) | [The Compressed Result](#the-compressed-result) | [Beyond Python](#-beyond-python) | [Challenge](#challenge) | [Summary](#summary)

## Introduction

> &#128214; Proverbs 16:11 - A just balance and scales are the LORD’s; all the weights in the bag are His work.

In this lesson we are going to learn how to compress our projects into a single compressed file. This will be very useful for us because files like Python files cannot be directly emailed to other users, or loaded onto other systems because of hackers and others who write _malicious code_. Therefore, we are going to learn how to compress our files for the purposes of saving space on our computer system, and safely emailing our files to our instructor.

> **Malicious Code**: Is any code or script written for the purpose of exploiting another person's computer system, or personal information for the unjust gain of another person or persons.

Remember, the God of the old testament is the God of the new testament. God is immutable, He does not change. (Malachi 3:6) Therefore, the God who loves just weights and balances (integrity of heart) in the book of Proverbs is the same God who gave us His beloved Son Jesus Christ for our sins.

## Create An Empty Project

The first thing we are going to do is create an empty project for the purpose of learning how to compress the project into a single file.

**Step 1:** Open VS Code and then open an integrated terminal.

**Step 2:** Use what you learned from a previous lesson and navigate to your `Desktop` folder on your computer, in your terminal window.

_Example: On many systems, the following command works: `cd ~/Desktop`_

> The `~` is the shortcut symbol for the `home` directory.

**Step 3:** Use the `mkdir` command to make a new directory named `my_project`

**Step 4:** Now use the `cd` command to navigate into the `my_project` folder.

**Step 5:** Create five empty Python files using the `touch` command.

`touch python_file_{1..5}.py`

**Step 6:** Now use the `ls` command to verify that the files were created.

**Step 7:** Now use `cd` and the `..` to go up one level back into the `Desktop` folder.

![the commands](../images/0.7%20commands.png)

## View the Contents

Now we want to view the contents of the `my_project` folder from a GUI perspective. **GUI** (goo-ey) stands for **graphical user interface**. The GUI is the standard Windows/Mac/Linux environment you are use to with all the windows and file icons that you click on every day. 

### Open the `my_project` folder

Double click on the `my_project` folder to view your files.

![view your files before compressing](../images/view%20files%20before%20compressing.png)

### Compress in Windows / Linux

In Windows, right click on the folder to be compressed and select `Send To` and then select `Compressed (Zipped) Folder`

![compress in Windows](../images/compress%20on%20windows.png)

### Compress in MacOS

In MacOS, right click on the folder to be compressed and select `Compress`

![compress on Mac](../images/compress%20on%20mac.png)

### The Compressed Result

The final result will be a compressed **zip** file. The zip file will have the `.zip` extension. A zip file is a file that has been compressed and reduced in size. Just how much a file or set of files compress depends on the type of files you have, their contents, and the compression algorithm (set of rules) your computer system uses to compress its files.

![compressed file](../images/0.7%20zippped%20project.png)

That's it! End of lesson!

## Challenge

Eat a cookie. Hug someone you love. Show love someone today who may be difficult to love. Give God the glory in Jesus Christ. That is your challenge today! ... Mine too. :smiley:

## Summary

In this lesson we have talked about how to use our operating systems built in data compression abilities. This creates what is called a _zip_ file. A file that is compressed. A compressed zip file can contain one file, or multiple files with multiple folders. This data becomes encrypted and unreachable until it is then decompressed. In the next lesson we will talk about _uncompression_ or _extraction_.

---

**Projected Lesson Read Time: 8 minutes**

&#8678; Previous Lesson: [Navigating Your Computer](./006_navigating_your_computer.md)

&#8680; Next Lesson: [Extracting Files](./008_extracting_files.md)
