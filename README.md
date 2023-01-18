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
- <b>$ git rebase 'Branch Name'</b>  
<br><br>

## Change commit message -
- The <b>'git commit --amend'</b> command allows you to change the most recent commit message.
#### Steps : 

- 1] Navigate to the repository directory in your terminal.<br><br>
- 2] Run the following command to amend (change) the message of the latest commit:<br><br>
   - <b>git commit --amend -m "New commit message."</b><br><br>
   - What the command does when run, is overwriting the most recent commit with the new one.<br><br>
- 3] If you changed the commit message than you push commit to the branch.<br><br>
<br>

## Cherry pick commit -
- With the <b>"cherry-pick"</b> command, Git allows you to integrate selected, individual commits from any branch into your current HEAD branch.<br><br>

- For Example, Git cherry-pick is helpful to apply the changes that are accidentally made in the wrong branch. Suppose I want to make a commit in the master branch, but by mistake, we made it in any other branch. then we will use git cherry-pick command.<br><br>

- Copy the particular commit id that you want to make on the master branch. Now switch to master branch and perform This command :<br><br>
  - <b>$ git cherry-pick '<commit id>'</b> <br><br>
  - with git cherry-pick command and made that commit into my master branch. You can check it by <b>'git log'</b> command.

<br><br>


## Drop Commit Massage -


