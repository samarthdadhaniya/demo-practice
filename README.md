# Git Basic Commands

- Create one repository called demo-practical and perform below task :

## Pull-Request and Merge -
#### Steps : 

- 1] Switch to the branch that you want to create a pull request for.<br><br>
- 2] Click Create Pull Request. GitHub Desktop will open your default browser to take you to GitHub.<br><br>
![windows-create-pull-request](https://user-images.githubusercontent.com/71020225/213085619-9cafbfae-ed98-4a2e-b271-2292cf53922a.png)

- 3] Type a title and More About Your Pull-Request for your pull request.<br><br>
![pullrequest-description](https://user-images.githubusercontent.com/71020225/213086236-b892fd34-b080-428e-ac3a-7750f2a0faac.png)

- 4] To create a pull request that is ready for review, click Create Pull Request, use the drop-down and select Create Pull Request, then click Pull Request.<br><br>
![pullrequest-send](https://user-images.githubusercontent.com/71020225/213087160-b598c8cf-f723-4e8e-aa47-dfb9e555211a.png)
<br><br>




## Git Rebase -
- Rebase is one of two Git utilities designed to integrate changes from one branch onto another. Rebasing is the process of combining or moving a sequence of commits on top of a new base commit. Git rebase is the linear process of merging.<br>
![Git_Rebase_1](https://user-images.githubusercontent.com/71020225/213090149-49f8562b-82e8-420d-8822-fedf6cd7504d.png)<br>

#### How to Rebase : 
- When you made some commits on a feature branch (xyz branch) and some in the master branch. You can rebase any of these branches. Use the git log command to track the changes (commit history). Checkout to the desired branch you want to rebase. Now perform the rebase command as follows:

#### Command :
```
$ git rebase 'Branch Name'
```  
<br>


## Change commit message -
- The ```git commit --amend``` command allows you to change the most recent commit message.
#### Steps : 

- 1] Navigate to the repository directory in your terminal.<br><br>
- 2] Run the following command to amend (change) the message of the latest commit:<br>
```
git commit --amend -m "New commit message"
```
   <br>
   - What the command does when run, is overwriting the most recent commit with the new one.<br><br>
- 3] If you changed the commit message than you push commit to the branch.<br><br>
<br>



## Cherry pick commit -
- With the ```cherry-pick``` command, Git allows you to integrate selected, individual commits from any branch into your current HEAD branch.<br><br>

- For Example, Git cherry-pick is helpful to apply the changes that are accidentally made in the wrong branch. Suppose I want to make a commit in the master branch, but by mistake, we made it in any other branch. then we will use git cherry-pick command.<br><br>

- Copy the particular commit id that you want to make on the master branch. Now switch to master branch and perform This command :<br>
```
$ git cherry-pick '<commit id>'
```
  <br>
  
  - with ```git cherry-pick``` command and made that commit into my master branch. You can check it by ```git log``` command.

<br>



## Drop Commit Massage -

- Generally, the ```git reset``` command is used for deleting the latest commits in Git, To delete the most recent commit, run the command below:<br>
```
git reset --hard HEAD~1
```
  <br>
  
  - To delete the ```N-th``` latest commits, you should use ```HEAD~N``` as the argument of git reset.
  
```
git reset --hard HEAD~N
```
  <br>
  
  - As an alternative to this method, you can select the appropriate commit by its hash instead of ```HEAD~N```, Here is how to do it:<br>
  
```
git reset --hard <sha1-commit-hash>
```



