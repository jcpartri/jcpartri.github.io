# The Terminal and CLI's


&#x2637; [Table of Contents](./../toc.md)

> **Disclaimer: The publish and/or author of this text is not responsbile for any damages received / given / or done upon your computer system from a faulty software installation or from a poorly written instruction. Make sure you know what you are doing before you proceed.**

The publisher and the author strongly recommend that you research your computer's system resources and all software documentation before installation. The author is not a licensed computer technician / software specialist and represents that they have no expertise in diagnosing, examining, or treating failed or damaging software installations of any kind, or in determining the effect of any specific damage on a given comptuer system.

You should understand that when installing any software, there is the possibility of physical injury to your computer. If you engage in this set of software installation instructions, you agree that you do so at your own risk, are voluntarily participating in these activities, assume all risk of injury to your computer / and/or the computer upon which the software is being installed, and agree to release and discharge the publisher and the author from any and all claims or causes of action, known or unknown, arising out of the contents of this book.

The publisher and the author advise you to take full responsibility for your computer system's safety and know your limits. Before implementing the software installation steps described in this book, be sure that your equipment is well maintained and do not take risks beyond your level of experience, aptitude, training, and comfort level.

## Lesson Outline

[WSL](#wsl) | [WSL Installation](#wsl-installation) | [Windows Powershell](#windows-powershell) | [VS Code's Integrated Terminal](#vs-codes-integrated-terminal) | [Beyond Python](#-beyond-python) | [Challenge](#challenge) | [Summary](#summary)

## Introduction

> &#128214; John 1:14 - And the Word became flesh, and dwelt among us, and we saw His glory, glory as of the only begotten from the Father, full of grace and truth.

When a user learns how to use a terminal application, that user has direct access to computer files and options. Think of it as a more personal, closer link between the user and the computer. Christ Jesus is our personal direct access to God. He became flesh, just as we are flesh, and He dwelt among us. God's goal in Christ is to bring us close to Him again. To have direct access to Him. This is of course way better than anything I could teach you about a computer terminal, but the parallel here does exist, so I want to take this time to capitalize on that parallel.

The terminal/command prompt is a CLI. CLI stands for **command line interface**. This was the first type of interface developed for users to interact with a computer system. The keyboard is the primary device used in a CLI.

![A Keyboard](../images/computer_keyboard.png)

We want everything we do in the CLI in this text to be consistent. Therefore, for Windows users, we are going to make sure that the commands we type in the terminal window work across all systems. Therefore, if you are a Windows user, we are now going to talk about using the PowerShell instead of the Command Prompt.

> ---
> If you are not a Windows user, but a MacOS or Linux user, you can skip this next section.
> ---

## WSL

This next section is **IMPORTANT** for Windows users, so pay close attention. 

We are going to try to install WSL on your system. WSL stands for "Windows Sub-system for Linux" The reason why we are going to try to install this is to make the process of going through this text easier for everyone. We will be able to standardize the commands given to all readers so that all commands will work whether you are a Windows / MacOS / or Linux user.

> Note: If you cannot get the WSL to install, do not worry. Take a deep breath. It will be fine. You can still get through this text and learn a lot. You will just need to pay close attention to differences given between Windows commands and MacOS/Linux commands as you proceed through the text.

As always...

1. Make sure you have the needed specifications on your computer before you install.
2. You must have Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11 to use the commands given.
3. You need to have the necessary permissions.
4. This will take TIME to install, so it is best to do this when no one else needs the computer. Maybe at 12 AM in the morning when people are sleeping. Let the install run through the night.

**Only proceed with WSL Install if you meet the specifications given above**

If you need to bypass WSL Installation then click on this link to go to the [PowerShell](#windows-powershell) section.

---

### WSL Installation

Click on the Windows search bar and type in: PowerShell. Select "Run As Administrator".

![Running PowerShell](../images/opening_powershell.png)

Click on the following link and follow the given instructions: https://learn.microsoft.com/en-us/windows/wsl/install

**If the installation worked! You do not need to use the Powershell! Congratulations!**

**If the installation did not work, then proceed to the section on the [Windows Powershell](#windows-powershell)**.

---

### WSL In the Integrated Terminal

1. Open VS Code
2. Select the `Terminal` menu from the top.
3. Select `New Terminal`. The integrated terminal should appear. The bottom panel is the integrated terminal. It may or may not look like this.

![Setting WSL](../images/setting%20WSL%20in%20the%20integrated%20terminal%20window.png)

_WindowsSauce is my terminal prompt. I set this myself. I will let you investigate how to change your terminal prompt on your own._

Do you see the new terminal button? ![new terminal button](../images/new%20terminal%20button.png) It looks like a plus sign with a drop down arrow. Select the drop down arrow and choose the version of Linux with the WSL next to it. My version is Ubuntu, but you can also install other versions of Linux. The WSL is the important thing.

That is it! You are done! This is the terminal you want each time you start VS Code!

You may now proceed to the [Beyond Python](#-beyond-python) section.

---

### Windows PowerShell

The Windows PowersShell is a more advanced CLI than the traditional command prompt. Even better, commands that are typed with regularity in the MacOS terminal and Linux terminal overlap with the PowerShell command set. This will make our lives a lot easier.

**Step 1:** Type in PowerShell in the Windows search bar. Run the PowerShell as an Administrator.

![opening powershell](../images/opening_powershell.png)

In the off chance that the PowerShell is not installed on your system, go to the following link and download and install the PowerShell. 

[Download and Install the Windows PowerShell](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4)

Here is the URL if the link above does not work: https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.4

**Step 2:** Once you open the PowerShell you should get a window that looks like the following. (Yes there may be differences).

![what the powershell looks like](../images/powershell.png)

Ok, now we know we have PowerShell on our system, but now we turn our attention to making it function as an **integrated terminal** in VS Code. Again, MacOS and Linux users do not need the next section.

## VS Code's Integrated Terminal

**Step 1:** Open VS Code. At the top menu select: `Terminal`. You should see the following drop down menu.

![new terminal](../images/vs_code_open_new_terminal.png)

Once you have opened a new integrated terminal a terminal "of some type" will open. It may or may not be the PowerShell. If it is, then Great! If not, then don't worry. Or goal is now to get VS Code to default to the PowerShell.

Your terminal window will have this basic look, but again, there will be differences.

![first open terminal](../images/integrated_terminal_in_vs_code.png)

Do you see where it says `WindowsSauce`. This is my own personalized prompt. Yes, you can customize your own. No I will not show you how. :-P.

Now above this window is a little bar that has some or all of the following items on it.

* Problems
* Output
* Debug Console
* Terminal
* Ports
* etc...

You will notice that to the right and at the top, you can see that it states: `pwsh`. This is how I know I am using the PowerShell. If yours also says `pwsh`, then you are good to go.

Notice that there is an icon that has a plus sign and a drop down arrow. ![new terminal button](../images/new%20terminal%20button.png)

If you click on the drop down arrow, a list of possible CLI's will present themselves to you.

![terminal drop down menu](../images/terminal_drop_down_menu.png)

**Select:** `PowerShell`.

Now if the PowerShell does not exist in your drop down menu, don't panic. You can get this to work. Maybe you need another source however, therefore here is a link that will redirect you to the VSCode Site

https://code.visualstudio.com/docs/languages/powershell


## &#x2708; Beyond Python

I think you are going to like this challenge. :smiley: It's called [**Terminal Tutor**](https://www.terminaltutor.com/) it will help you learn the basics of typing commands in a Unix based terminal. MacOS is built on top of Unix, and Linux looks very much like Unix.

> Note: If you were not successfull in the installation of WSL (given above) then you may still go to this site and have fun with it, but there are commands you will learn that will not be available in the Windows PowerShell. Bummer. :frowning:

Terminal Tutor: https://www.terminaltutor.com/

## Challenge

The following link on [Terminal Basics](https://code.visualstudio.com/docs/terminal/basics) might be useful to you as you begin to uderstand what the terminal is and how to use it.

**Warning!:** Don't break your system! Be very careful about trying new features in the terminal because the terminal has access to critical files on your comptuer and it is VERY easy to do something un-intelligent in the terminal if you do not know what you are doing.

## Summary

At the beginning of this lesson we looked at John 1:14 and made a parallel between Christ as our access to God and the terminal as a user's direct access to a file system. There is a great contrast however.

A user will want access to a file system in order to control that system and make changes to that system. This is not how our relationship with Father, Son, and Spirit works, however.

Christ as our direct access means we can finally relate to Him from a position of rest. We are no longer consumed by the demand for justice against our sins. (Romans 1:18, 3:25-26, 5:8) Christ has paid the penalty for us on the cross. Now, we have a rest in God and can know God and love God for the sake of knowing and loving Him. Love God, for God. This access is meant for relationship, not for control.

In this lesson we have learned the following

- CLI stands for command line interface
- The Windows PowerShell command set overlaps with the MacOS and Linus terminal command sets. This will make our lives easier by trying to develop a standard to work with from the very beginning.

---

**Projected Lesson Read Time: 8 minutes**

&#8678; Previous Lesson: [Opening, Naming, Saving Python Files](./004_opening_naming_saving_a_python_file.md)

&#8680; Next Lesson: [Navigating Your Computer](./006_navigating_your_computer.md)
