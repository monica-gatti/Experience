# Initialize a new project with git init  

In the local folder, from vscode terminal or cmd line:  
´´´
git init  
´´´
Starts a new local repository ( you will see the .git folder)  
´´´
git init subfoldername  
´´´
Starts a new local repository in a subfolder  

After creating the new local repository, you can create files, make change  
Add the changes using:  
´´´
git add filename  
´´´
Commit the change using:   
´´´
git commit -m "your comment" filename1, filename2   
´´´
Add the remote URL to your local git repository: this assign the name origin to your local repository  
´´´
git remote add origin <GITHUBPROJECTURL>  
´´´
Now you can push the changes of the commit  
´´´
git push -u origin main  
´´´
Note that the -u flag creates a tracking reference for every branch that you successfully push onto the remote repository. 
The local branch you push is automatically linked with the remote branch. This allows you to use commands such as git pull without any arguments.  

See https://github.com/git-guides/  
