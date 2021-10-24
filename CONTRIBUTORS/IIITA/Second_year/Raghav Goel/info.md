Merge Conflicts arise when commits are added to the same place in a file, when they coincide.Suppose both the commits want to add changes to the same line, they are not overwritten by each other, and hence merge conflicts arise.
Hey!<br>
This is Raghav Goel.<br>
My  <a href = ""https://github.com/raghavgoel25"">Github Profile</a>

What do you really understand from SSH keys? What are the advantages of using it?

SSH key is a method that can be used for authentication different from normal passwords mainly in the way it operates. 
SSH keys are more long than typically used passwords and are computer generated, making them less prone to hacking. 
 They are not stored on servers, but only the device which is being used for login, hence again
making it less vulnerable to hacking.
 
 How to edit the last commit message in git?
 The following commands should be executed:-
 1.git commit --amend -m "New message" 
 2.git push --force repository-name branch-name
 If you are not sure whether someone has cloned your repository after your latest commit, instead of the second command, us
 git push --force-with-lease repository-name branch-name
 This command will abort the push if there are any upstream changes to the repository, whereas the --force command will destroy any changes.


 How to delete a commit?
 I will use git reset --hard HEAD^ to delete the latest commit i will have made.
 
 WebD


OnlineResources
https://www.udemy.com/course/the-web-developer-bootcamp/
Force push is generally not advisable. Suppose it is a common repository with many people working on it, force pushing, when changing the history of the remote can lead to other users being out of sync and not being able to collaborate properly. It was okay for use to do it because we alone worked on our repositories.

Reordering a Commit.
Title- Reodering a Commit
Description:
In your main branch ,answer two questions. Q1)Why would one ever need to ever reorder his commits? Q2) Is reordering your commits a good practice? If not, when?
Commit these changes.
Make a new branch now.Split this commit into two commits. 
Make another new branch, and cherry pick these commits. 
Now reorder these commits so that the commit for Q2 is before the commit for Q1.Push these changes,and make a PR. 
Now when you go to the PR, you may find that the order of commits shown there is not the order you had set. Find out why. Answer this as Q3, and commit this change too. 
NOTE: The total number of commits on the PR should be 2 only ;)
