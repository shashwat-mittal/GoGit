ans-1 : it arises when git cannot merge changes automatically. like while doing the cherry-pick task, we faced merge conflicts because while cherry-picking we changes the text in the same lines and git cannot understand which change to  preserve while merging. 

### Hey, I'm Varun Tiwari
I am a student of ABV-IIITM, Gwalior.
To know more about me [visit here](https://github.com/varunKT001)
This is the link of the repo [GoGit_repo](https://github.com/varunKT001/GoGit)

## Issue : 223 
#### Ques - What do you really understand from SSH keys? What are the advantages of using it?
SSH keys are just pairs of a public and private key. The Private keys are used to encrypt/decrypt the user identity. SSH keys provide more security as well as convinience to the user.  

## Issue : 332 
#### Ques - How to edit the last commit message in git?
There are two cases : 
1. Changes not pushed : If changes are not pushed we can simply add --amend flag and it will amend last commit. 
2. Changes are pushed : If Changes are pushed we need to --amend the and also force push the changes using the -f flag

## Issue : 366
First commit. We will go to the file state in first commit and checkout to new branch. then we will come to master and hard reset to the previous branch head.

ans-2 : yes. force pushing is bad practice because it modifies git history and lead other users become out of sync. We may overwrite someone else's commits and cause merge conflicts for others. It did'nt cause any problem in our case because we were the one working on our repositories.  
ans-3 : I think the git bisect isn't used in any task. 
top commit : If we had all the three ans at the end of the file, we would need to manually edit the hunks to only contain one answer and then commit the changes.




web developement









youtube: freecodecamp


so first I used git log to see the last commit on 14 october because we know that no bug was there at that time
Then I copied the commit hash of the last commit of 14 october and used: 
git bisect start HEAD <commit hash>
This starts git bisect and test each commit for a bug. we will use
git grep 'bug'
this will find all files by matching if file contains 'bug'.
If we do not find a file we will tell bisect to mark the commit as good: 
git bisect good
But if we find the file with bug, we will use
git bisect bad
Upon finding a bad commit, git puts us on the same commit we marked bad
then we can copy the commit hash and use
git bisect reset
This will put us on the head from where we started
Now we can revert the changes of the bad commit using 
git revert <bad commit hash>
This is the best method to find bug because we can move to individual commits and test the code for bugs and can revert the changes if bug is found. 











