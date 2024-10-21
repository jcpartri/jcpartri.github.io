# Chapter Review

&#x2637; [Table of Contents](./../toc.md)

What have we learned so far? Let's go through our vocabulary word database first and refresh our memories.

## Vocabulary

- IDE: Integrated Developers Environment
- root folder: The primary or base folder where project files in VS Code are located
- folder heirarchy (also knowns as file tree) is the structure or arrangment of files and folders on a computer system
- .py extension: All Python files must end with the .py extension
- CLI: Command line interface. Examples of this are MacOS/Linux Terminal, Windows Command Prompt, Powershell, and VS Code Integrated Terminal
- GUI: Graphical user interface
- File System: A set of files and directories that are interconnected in the form of a tree. All files and directories on a systme are tied into the root
- absolute path: a path in a file system that is directly connected to the root
- relative path: a path in a file system that is relative to the users current working directory
- malicious code: any code or script written for the purpose of exploiting another person's computer system, or personal information for the unjust gain of another person or persons.
  
### Terminal Commands

- `pwd`: print working directory
- `ls`: list contents of the current working directory
- `ls -a`: list all contents, including hidden files, of the current working directory
- `*`: the wildcard character
- `cd`: change directory command
- `..`: go back one level in the current path
- `.`: the current working directory
- `CTRL + L`: use this key combination to clear the screen in the terminal window
- `touch`: a command that updates the timestamps of a file or directory. If the file does not exist, then the touch command creates an empty file with a new timestamp
- `mkdir`: the make directory command

## Quiz

1. **Which path below is an absolute path?** Paths may alternate between Windows, MacOS, and Linux.
   
   - [ ] `./documents/work/office`
   - [ ] `Documents\Work\Office`
   - [ ] `../office`
   - [ ] `C:\\Users\username\Documents`

2. **What is the BEST answer that describes the meaning of the following command?**

   `mkdir ../office`
   
   - [ ] make a new directory named office
   - [ ] make a new directory in the working directory named office
   - [ ] go up one level in the file system and create a new directory named office
   - [ ] make a new directory named ../office

3. **Given the file tree below, which command will help you navigate into the temp folder?**
   
   Assume the `images` folder is the current working directory.

   ```console
   main_project/
   ├── images/
   │   ├── image1.png
   │   └── image2.png
   ├── main.py
   ├── README.md
   └── temp/
      ├── update.py
      └── resource.txt
   ```

   - [ ] `mkdir ../temp`
   - [ ] `cd ../temp`
   - [ ] `cd C:\\Users\\username\Documents\main_project\temp`
   - [ ] `cd ./temp`

4. **Choose the answer that you think might BEST summarize the following scenario.**

   Audrey knows how to program her computer system. She wants to see if her brother has been logging into her web browser on her computer, so she writes a short script that keeps track of logins to that browser, the time of login, and who logged in.
   
   - [ ] Audrey has written malicious code
   - [ ] Audrey has not written malicous code
   - [ ] Audrey has done something questionable
   - [ ] What Audrey has done is neither right nor wrong

5. **Choose the answer that you think might BEST summarize the following scenario.**
   
   Maxwell's parents have agreed to pay $50 each month to a local ministry. For the past three months, his parents have been extrememly busy at their workplace and have fallen behind on managing their finances. In other words, they forgot to honor their agreement to the ministry. 

   Maxwell's mom always writes down her passwords on a sticky note in her office and he knows the website for their banking institution. Maxwell decides to help his parents out and log into the banking site so he can transfer the monies they forgot.

   - [ ] Maxwell has decided to do it, but he hasn't done it yet, so nothing un-ethical has been done here
   - [ ] This is a potential disaster waiting to happen
   - [ ] Maxwell's intentions are good, but his actions are questionable
   - [ ] Maxwell needs to call the ministry and explain why the donations for the past three months have been delinquent

6. **The command `pwd` stands for...**
   
   - [ ] print working directory
   - [ ] please wait downstairs
   - [ ] pirates won't dance
   - [ ] print working data

7. **Which of the file names below will make the file a 'hidden' file on a computer system?**
   
   - [ ] hide_you_can_see_me.txt
   - [ ] ./you_can_see_me.txt
   - [ ] _hidden_file.txt
   - [ ] .you_can_see_me.txt

8. **The following command will NOT work in the terminal window.**
   
   `touch touch`

   - [ ] True. You cannot create a folder with the same name as a command.
   - [ ] True. You cannot write out a command twice.
   - [ ] False. It creates a directory named touch.
   - [ ] False. It creates a file named touch.

9.  **What will the following command do?**
   
   `cd ../..`

   - [ ] The command will go up the file system path two levels.
   - [ ] An error will occur
   - [ ] The command will go up on level in the file system and then go into a folder named `..`.
   - [ ] Nothing will happen.

10. **Follow the given directions carefully, then answer with what you think is the BEST choice.**

   Open your VS Code and then open an integrated terminal.

   **For Windows Users - type:** `py -m pip install cowsay`

   **For MacOS and Linux Users - type:** `python3 -m pip install cowsay`

   After installation type: 
   
   `cowsay -t "Let everything that has breath, Praise the LORD"`
   
   - [ ] This is an udder disaster
   - [ ] ASCII Cow lives!
   - [ ] I should milk this for all its worth!
   - [ ] Mooo.


&#8678; Previous Lesson: [Extracting Files](./008_extracting_files.md)

&#8680; Next Lesson: [Challenge Problems](./010_challenge_problems.md)
