# GitHub Live Demo Workshop
*Setup a Python script to fetch levels from CDA with **emphasis** on using git/github*

**Demo Notes**: ⚠ Disable camera 📷, it will cover the code

## Part 0 - Setup for Both Gui/Terminal
*Initial Setup for VSCode/Git*

1. Install Git (through IT/Online)
2. Install VSCode (IT/Online) and open/launch VSCode
3. Click "File" > "New Window"
4. Click "File" > "Open Folder"
   1. Navigate to where you want your project to live (or where it already lives)
   2. Select the folder you want git to be initialized from
5. (Do ONCE) Setup Git Environment for System
   1. Click "Terminal" > "New Terminal" from the menu bar
   2. In the terminal that opens replace name and email with yours and type these lines, pressing enter after each:
      1. `git config –global user.name "First Last"`
      2. `git config –global user.email "first.m.last@domain.com"`


## Part 1 - Using Git with Terminal
*A complete walk through on using git in the terminal for this project (and others)*
1. Open command prompt/terminal
2. Navigate to your project directory
   * **⚠ Shortcut / QOL!**  
     1. Right click in the blank space under your project folder name
     2. Select "Open in Integrated Terminal"  
     This will keep the terminal inside VSCode and save you on `alt+tabbing`
   ![Open terminal for this directory](resources/images/terminal_shortcut.png)
3. If you did not chose the integrated terminal you can type:  
        `cd C:\path\to\your\project\`   
        *Be sure the final directory is the root of your project!*
4. ⌨ Initialize the repository
   1. type  `git initialize` in your terminal
   2. Press enter! 


## Part 2 - Using Git with the VSCode GUI
*A complete walk through on using git in the VSCode GUI for this project (and others)*
1. Initialize your Local Repository
   1. Click the "Source Control" button:
   ![Source Control](resources/images/source_control.png)
   2. Click "Initialize Repository" or "Publish to GitHub" (*if you know that you want this project to have a remote repository*)
    ![Initialize or Publish](resources/images/init_repo.png)
2. If you have any changes you will see them now with a blue "commit" button, otherwise you will see a "publish" button

## Part 3 - Collaborating with Others

## Problems
1. ### Where is my menu bar?  
   *There are a few different styles for the menu bar in VSCode.*
   * Sometimes it is the burger menu (3 horizontal lines)
   * In others it is horizontal text across the top of your VSCode window  
**To Change it:**
     1. Click the ⚙ Gear icon at the bottom left 2. Select "Settings"
     3. Type "menu" in the search
     4. Scroll down until you see "Menu Bar Visibility" 
     5. Select whichever option suits you (i.e. `classic`) 
        ![Alt text](resources/images/menu_screenshot.png)  






Show how to see if git is installed (terminal)
Setup Git Environment
Initialize Repo
- Create .gitignore
	https://github.com/github/gitignore/blob/main/Python.gitignore
- Create README.md
Add our code, make changes
Commit
Make some more changes
Commit

- Show local .git - i.e. local vs remote
- Show git graph and our changes

Create a branch named "add
