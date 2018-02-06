# hardware
Schematics and layout work 


## Getting started with git
the main workflow is usually like this:

1. install git on your machine https://git-scm.com/download/
2. use the git bash terminal window to work with the repositories:
3. clone the repository of choice: in your terminal window, navigate to the folder you want to store the repository in, and send the command **git clone** **https://github.com/sfuphantom/hardware.git** for the hardware repository for example
3.5 the hardware repo has folders that contain a submodule - which is essentially just a version of a different repo, nested inside the hardware folder. this nested repo is the altium-libraries repository! to enable it, use **git submodule init** while in the hardware directory, and then **git submodule update**
4. now if you navigate to that folder in your normal file browser, you should see the repository folder with all the files in it
5. you can now edit the files and add new files into the repository folder like normal, as you would any folder system
6. to register new added files you have placed in the repository folder in your file browser, use the command **git add -A** in your terminal window while in the directory of your repository (**cd /documents/phantom** will change your active directory to /documents/phantom, and **cd ..** will change your active directory up one level)
6.5 **git add -A** will add all new files repo folder to be tracked by git
7. to save the changes you have made and the files you have added, use the command **git commit -m "fill in your update here"** to commit your changes and save them with a useful message
8. when you are ready to update the centralized repository on github with your changed localized cloned repository, use the command **git push** and you should see your changes show up on github

http://rogerdudler.github.io/git-guide/

https://learngitbranching.js.org/

http://www.ndpsoftware.com/git-cheatsheet.html#loc=workspace
