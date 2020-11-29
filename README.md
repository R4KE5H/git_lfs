# Git LFS

How to git push large files to github!!...

Do you know how to git push large files to github? This post will be helpful for you to push larger files in github.

When I tried to git push this “ratings.csv” file into my Github repo, it throwed some error because the file was larger than 100 mb. It was really annoying, and eventually i got to know about Git LFS an open source to push large files to Github by using few commands.

So how do we push large files like audios, videos, datasets and graphics to GitHub?  

"An open source Git extension for versioning large files"

"Git Large File Storage (LFS) replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git"

# How to get started with Git LFS?(This is what i did..)

1.Download and install the Git command line extension. Once downloaded and installed, set up Git LFS for your user account by running.

 -> git lfs install (Note:You only need to run this once per user account.)

2.Firstly,Remove your large file from your local repo directory BEFORE you set tracking for Git LFS. And Git push the local repo to Github as you use to push.

3.Secondly, Place the larger files inside your local repo that was pushed earlier.

4.Thridly, In the Git repository where you want to use Git LFS,select the file types, for example use this command which is given below(according to your file types).

For example:
-> git lfs track "*.psd"

 NOTE: Now make sure .gitattributes is tracked.

For example:
-> git add .gitattributes

5.Finally, you can just commit and push to github as you normally would.


Reference: 
https://git-lfs.github.com./, 
Dataset - https://www.kaggle.com/rounakbanik/the-movies-dataset?select=ratings.csv, 
https://github.com/R4KE5H/git_lfs




Thank you! Have a great day...
