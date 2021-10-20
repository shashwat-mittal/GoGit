Hello! This is Aviral Gupta. I am a 3rd year student at IIITA.<br>
Repo URL: https://github.com/aviralgupta752/GoGit.git

<b>What do you really understand from SSH keys? What are the advantages of using it?</b>
SSH(Secure Shell) keys are an access credential that us used in the SSH protocol. While working with github, we need to verify ourselves using our username and password. SSH key is an alternative way to verify ourselves.
SSH keys are more difficult to hack than passwords and thus are more secure.

<<<<<<< HEAD
To edit the last commit message one must use ```git commit --amend``` comand.
=======
To edit the last commit message one must use ```git commit --amend``` comand.

# Issue 336
first commit

second commit:
Steps:
I have removed the first commit.
Step 1: Finding the commit before the first commit using git log
Step 2: Checkout that commit using git checkout
Step 3: Make a new branch using the current checkout commit git checkout -b new_branch
Step 4: Adding the commit after the removed commit git cherry-pick
Step 5: Resolving merge conflicts and pushing our changes.
Step 6: Double checking everything using git status.
Step 7: Finally, switching to the original branch and performing a hard reset to the commit prior to first_commit using git reset --hard
Step 8: Merging new_branch using git merge new_branch
Step 9: Force pushed the changes in the repo using git push --force origin main
>>>>>>> a34788c (second commit)

<b> Ques - 1 Which kind of development(s) do you do? (web/app/cc/etc).</b>

Competitive Coding.

<b>Ques - 2 Resources that you follow to learn the above tech-stacks (development)?</b>

Youtube, GFG for concepts and leetcode, codechef for practice.
