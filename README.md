This a lesson using Bootstrap 3.3.7
This is a test to make sure I am updating with GitHub after migration

I had not set my name and email globally when i made a commit and it made Ubuntu the author of the commit.
I tried to change it using the following code:

'''  README.md

nothing added to commit but untracked files present (use "git add" to track)
vocstartsoft:~/environment (master) $ git add .
vocstartsoft:~/environment (master) $ git commit -m "adds RREADME.md"
[master 87b662f] adds RREADME.md
 Committer: Ubuntu <ubuntu@ip-172-31-43-89.ec2.internal>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 2 insertions(+)
 create mode 100644 README.md
vocstartsoft:~/environment (master) $  git config --global user.name "HelenSayer"
vocstartsoft:~/environment (master) $  git config --global user.email helen.sayer10@gmail.com
vocstartsoft:~/environment (master) $ git commit --amend --reset-author
hint: Waiting for your editor to close the file... fatal: cannot run /usr/bin/nano: No such file or directory
error: unable to start editor '/usr/bin/nano'
Please supply the message using either -m or -F option.
vocstartsoft:~/environment (master) $ git commit --amend --author="HelenSayer <s.com>"                                                                                                                            
hint: Waiting for your editor to close the file... fatal: cannot run /usr/bin/nano: No such file or directory
error: unable to start editor '/usr/bin/nano'
Please supply the message using either -m or -F option.
vocstartsoft:~/environment (master) $ git commit --amend --author="HelenSayer <helen.sayer10@gmail.com>"                                                                                                          
hint: Waiting for your editor to close the file... fatal: cannot run /usr/bin/nano: No such file or directory
error: unable to start editor '/usr/bin/nano'
Please supply the message using either -m or -F option.
vocstartsoft:~/environment (master) $ git commit -m "adds me as author to this commit as was not set after import to AWS Cloud9 after cloning from GitHub to new ASW environment"
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
vocstartsoft:~/environment (master) $ git push
Username for 'https://github.com': HelenSayer
Password for 'https://HelenSayer@github.com': 
Counting objects: 3, done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 451 bytes | 451.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/HelenSayer/whiskey-drop-bs3.git
   7819561..87b662f  master -> master
vocstartsoft:~/environment (master) $ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
vocstartsoft:~/environment (master) $ git '''
