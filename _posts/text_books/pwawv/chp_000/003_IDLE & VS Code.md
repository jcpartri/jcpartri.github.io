# IDLE & VS Code

&#x2637; [Table of Contents](./../toc.md)

## Lesson Outline

[Opening and Understanding IDLE](#opening-and-understanding-idle) | [The Shell](#the-shell) | [The Editor](#the-editor) | [VS Code](#vs-code) | [Working From A Project Folder](#working-from-a-project-folder) | [Beyond Python](#-beyond-python) | [Challenge](#challenge) | [Summary](#summary)

## Introduction

> &#128214; 2 Timothy 2:21 - Therefore, if anyone cleanses himself from these things, he will be a vessel for honor, sanctified, useful to the Master, prepared for every good work.

I think 2 Timothy 2:21 is a good verse for this lesson. We are getting things prepared on our computer systems so that we can learn about the exciting things code can do to solve problems. We want to prepare well. Notice that the verse above begins with _Therefore_. This means that something has been stated before. Go ahead and look up what those things are for yourself. 

If the apostle Paul speaks to us about cleansing ourselves from those things mentioned before, then we will be a vessel for honor, set apart, useful to our Master, and prepared for every good work. Even programming. :smiley: Do we desire to be vessels of honor, useful to our Master Jesus Christ? That is a question we all have to answer.

In the previous lesson you downloaded Python onto your system. When you did so, you also downloaded another application known as IDLE.

IDLE is a low-level IDE. IDE stands for **integrated developers environment**. Basically it is a text editor with extra fearures for code developers. IDLE is a good _beginners_ IDE with some nice basic features, but in this text we are going to want something more powerful than IDLE.

The recommendation of this text is to download and install VS Code. VS Code has many more advanced and easily usable features that IDLE does not provide for us. Before we download and discuss VS Code however, we will begin by discussing IDLE.

## Opening and Understanding IDLE

### Windows Users ![windows logo](../images/win11_logo.png)

In the Windows search bar below, type: IDLE. If everything installed successfully from the previous lesson, you should see something like this appear.

![windows IDLE app](../images/win_IDLE_app.png)

Click on the app and it will open.

### MacOS Users ![apple logo](../images/apple_logo.png)

Open spotlight search with the `Command + Space` keys and type in `IDLE`. If everything installed successfully from the previous lesson, then you should see something like the following.

![mac IDLE app](../images/mac_IDLE_app.png)

Click on the app and it will open.
 
### Linux Users ![tux](../images/my_tux.gif)

> Underlying Assumption: You are using a Debian based system like Ubuntu or Linux Mint.

To open an application in Ubuntu, type: `Alt + F2` then type in IDLE

To open a terminal window in Linux Mint type: `CTRL + ALT + T`, then type `idle &` (sometimes you will have to type `idle3 &`)

## The Shell

IDLE has two primary types of windows used for coding in Python. The **Shell**, and the **Editor**. By default, IDLE opens in the Shell. If you see the following symbols `>>>` then you know you are in the Shell.

The `>>>` are called _chevrons_. This means that IDLE is waiting for one line of user input from you. Once you have the IDLE Shell open, try typing in the following line, then hit the `Enter/Return` key.

```python
>>> print("Hello world!")
Hello World
>>>
```

Congratulations! You just typed your first line of Python code. Notice the output to the print statement appears immediately after the line you typed. Notice further that the output line does not have any chevrons. This is one way that you can know the difference between input and output in the Shell.

One of the drawbacks of the IDLE Shell is that you cannot go back and edit a line once you have typed it. This is rather a serious downside since if you make a mistake you have to begin again. Another drawback is that there is no real way to clear the screen once you reach the bottom. You either have to just keep typing from the bottom, or open a new Shell window. I personally find this feature rather frustrating.

![Bottom Line of the Shell](../images/bottom_line_in_Shell.png)

In summary, think of the Shell as a type of _calculator_ for Python code. Code is typed into the Shell one line at a time and the results are immediately calculated. This is fine for simple programming needs but the majority of the time you and I will need to write a program in block form, test it, edit it, run it, and then repeat that process until it works just right. This is where the IDLE Editor comes into play.

### Closing the Shell

To close the Shell, you can either close IDLE completely, or in the Shell type `exit()` to exit the Shell. However, keep the Shell open for now so you can go to the next topic.

## The Editor

In the next lesson I show you how to create a Python file and save it. But for now, let me show you how to open the Editor window. It is pretty easy.

Once you have the Shell window open, Go to the `File` menu at the top left of the window.

> **Note:** Mac Users: The file menu will be at the top of your screen rather than in the Shell window itself. _Apple prefers to give its users access to menu items through the menu bar at the top of the screen, rather than in an application window._

Choose `New File` and the Editor window opens. _That is it!_.  It is possible to tweak IDLE so that the Editor window opens by default rather than the Shell, but I will leave it to you to investigate how to do that on your own.

![IDLE Editor Window](../images/idle_editor_window.png)

Notice now that there are no chevrons `>>>`. There are line numbers however. If you have an older version of IDLE and you don't see line numbers there is a way to turn them on by going into `Options`, but I recommend you just download the latest version of Python.

We will talk more about the Editor in the next lesson.

## VS Code

If you have not already done so, download and install VS Code onto your system. Click on the link below or type the following address into your web-browser: https://code.visualstudio.com/download

[Download and Install VS Code](https://code.visualstudio.com/download)

Once VS Code is downloaded, double click on the installer file in your `Downloads` folder to install the application. An installation wizard should appear and you should select `Yes` or `Ok` to any menus that pop up.

### Opening VS Code

Whether you are using Windows, MacOS, or Linux, the VS Code app icon should look like the following image.

![VS Code Icon](../images/vs_code_icon.png)

In Windows type `Code` in the search bar.

In MacOS open spotlight search and type `Code`. 

In Linux press `CTRL + ALT + T` to open a terminal window, then type: `code &` and hit `Enter/Return`.

When VS Code opens you will see something like the following window. It may or may not be exactly like it.

![VS Code Getting Started](../images/vs_code_get_started.PNG)

## Working from a Project Folder

Once we are up and running and learning Python at a deeper level, you will want to be able to create your programs in a **root folder** of some kind. This will help organize your code and your projects so that they are not splattered all over your computer's hard drive. Lets discuss how you create a project folder. The process is very similar between all three platforms: Windows, MacOS, and Linux, so we will just show you the process in one platform. 

**Step 1:** In VS Code choose `File` and then `Open Folder`

![step 1](../images/working_from_a_root_folder_1.png)

_Linux Mint is the system I chose to use for this example. ... You are welcome! :smiley:_

**Step 2:** This next step may vary a little among systems. I am using Linux Mint in this example. Mint gives me a very nice `New Folder` icon to create a new root folder. Navigate to a location on your comptuer that you can remember and is a good place to store your project files.

> On MacOS ![apple icon](../images/apple_logo.png) and Windows ![win logo](../images/win11_logo.png), you can right click anywhere in the empty white-space of your window and select `New` and then `New Folder` or even just `New Folder` on MacOS.

![step 2](../images/working_from_a_root_folder_2.png)

**Step 3:** Since this is chapter_0 I named this folder `week_0`

![step 3](../images/working_from_a_root_folder_3.png)

**Step 4:** Select the `Open` button.

![step 4](../images/working_from_a_root_folder_4.png)

**Step 5:** You now have a root project folder! It's just that easy!

![step 5](../images/working_from_a_root_folder_5.png)

## &#x2708; Beyond Python

While I am currently typing this text, I am using VS Code and a root folder myself. Here is a quick gander at what my **folder heirarchy** looks like.

![folder_heirarchy](../images/textbook_folder_heirarchy.png)

## Challenge

Now that you know how to open the IDLE Shell, let's see how good you really are. :smiley:

Use the IDLE Shell and only the IDLE Shell to see if you can answer the following riddle.

_"I am an eighteenth century individual. In the year x squared, I was x years old. In what year was I born?"_

Here is a hint: To square something in the IDLE Shell type two asterisks. One asterisk will only multiply.

```python
>>> 4**2
16
>>> 5**2
25
>>>
```

Can you solve the riddle? Good luck!

## Summary

- IDLE has two primary windows for typing code in Python. The Shell and the Editor.
- Think of the Shell as a built in calculator for Python.
- Think of the Editor as an application like Notepad, or TextEdit.
- VS Code is a more advanced IDE that gives the developer many rich features to help develop software.
- Know how to create and open a root project folder in VS Code.

---

**Projected Lesson Read Time: 5 minutes**

&#8678; Previous Lesson: [Downloading and Installation of Python](./002_download_and_installation_python.md)

&#8680; Next Lesson: [Opening, Naming, Saving a Python File](./004_opening_naming_saving_a_python_file.md)
