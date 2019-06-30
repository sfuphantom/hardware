# hardware
Schematics and layout work 

## Getting started with git

Tutorial: https://www.youtube.com/watch?v=1xfp2Cx9FUk

the main workflow is usually like this:

1. install git on your machine https://git-scm.com/download/
2. use the git bash terminal window to work with the repositories:
3. clone the repository of choice: in your terminal window, navigate to the folder you want to store the repository in, and send the command `git clone` https://github.com/sfuphantom/hardware.git' for the hardware repository for example
4. the hardware repo has folders that contain a submodule - which is essentially just a version of a different repo, nested inside the hardware folder. this nested repo is the altium-libraries repository! to enable it, use `git submodule init` while in the hardware directory, and then `git submodule update`
5. now if you navigate to that folder in your normal file browser, you should see the repository folder with all the files in it
6. you can now edit the files and add new files into the repository folder like normal, as you would any folder system
7. to register new added files you have placed in the repository folder in your file browser, use the command `git add -A` in your terminal window while in the directory of your repository (`cd /documents/phantom` will change your active directory to /documents/phantom, and `cd ..` will change your active directory up one level)
8. `git add -A` will add all new files repo folder to be tracked by git
9. to save the changes you have made and the files you have added, use the command `git commit -m "fill in your update here"` to commit your changes and save them with a useful message
10. when you are ready to update the centralized repository on github with your changed localized cloned repository, use the command `git push` and you should see your changes show up on github

http://rogerdudler.github.io/git-guide/

https://learngitbranching.js.org/

http://www.ndpsoftware.com/git-cheatsheet.html#loc=workspace

## Branching

If you wish to work on a version of the repo without affecting or potentially causing conflicts, use **branches**. They are very useful for developing a new feature of a program/board without affecting the master branch. They can later be merged into the master branch by using a **pull request**. 
1. Navigate to your hardware directory in the git bash terminal window.
2. Use the following command `git branch MyBranchName` to create a new branch
3. Use the following command `git checkout MyBranchName` to switch your active branch to MyBranchName instead of Master
4. If you want to perform both commands in one line, here's a shortcut: `git checkout -b MyBranchName`
5. Now you can develop and make changes as you wish on MyBranchName, adding files, making commits, and pushing up to the repository held in Github. 
6. When you have decided you are ready to combine your changes/additions to the master branch of the repository, use Github's web interface (https://github.com/sfuphantom/hardware) to create a **new pull request**.
7. A pull request will alert other people that you are ready to combine your branch (MyBranchName) with the Master branch, and will allow them to review your work and approve it for merging. 
