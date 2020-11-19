# GithubExercise
Github Playground

Hi, this is a minimal github exercise to help you get familiar with git especially the github. 

Git is a program and a method to manage the version of your work (like codes, docs and so on) and cooperate with others. Github is a wonderful web site that helps you manage and perform the git command in the web page. So we first start with the Github.

## Basic github operation (need type in no command!)
Find the following after you registed the github account.
- [ ] "Fork" this repo. **"fork"** means you copy this repo and have full control to edit this as you like. **"repo"** means repository, like this "GithubExercise". You work in a repository and put related things (codes, docs, pictures and so on) in one repository like one project folder. You can have as many repos as you like in your github account or have local repos (will mention in next chapter) in your computer which are not uploaded. You can of course create your own repo but now we start with this existing one.
- [ ] Edit this readme file in github and do whatever you want like. Github provides simple editor that helps you edit the code and text online.
   - tick the tickbox 
   - put your nickname here: ???
   - add your comments
   - correct the grammar or other typos
- [ ] Commit your change. That is a snapshoot of one version. You can then edit other places and commit again. Different commits help you "seperate" different edit, like first commit you fix one specific bug followed by next commit adding one new funciton or feature. Mix every things in one commit is not good (except first initial commit). And later you will learn how to change to any version and debug the codes commit by commit.
- [ ] Then you can submit "Pull Request" to inform the original author (where you fork from) that you have some important change to submit and to let everyone know. Then the author will "pull" your changes and "merge" your changes to his repo so that, everyone fork his repo will see this and then "merge" with his edit. This related to how you cooprate with other contributors. The basic workflow is all of the contributors focus on one **"common"** or **"base"** or **"official"** repo (we will call the common repo all the people fork from, *"official"* repo in the following), and then fork->edit->commit->pull request, integrate all the changes and sync with all the contributor.
- [ ] How if you want to check and sync others' changes? Like you just found the "official" repo changed a lot after your fork and you hope to use the latest version of the "official" repo. 
   - First you look at the commit history of the *"official"* repo and be clear how it changed. (Also you can look at the history of your repo if you forget what you have changed after a long time of just want to debug). The most important information in the history is the commit id, it can be used to locate any version in the history.
   - Then you can submit a special Pull request, by reversing the direction and pull from the *"official"* to your repo. Then you will recieve the request sended by yourself and just agree to merge. Then your repo will be merged with the latest changes from the *"official"* one.
- [ ] How if you want to communicate inside the github like a pro? Use "Issue" of github and that means the author will see the message you post and to reply inside github. Find this and issue something to my this repo.
- [ ] How if you don't want to submit some part of your changes to the *"official"* one like you are doing some development only in your repo or not want to share or still in testing. You have many methods yo do this, but I would suggest you use the "Branch". The branch means a parallel version of your work, you can "branch" another version at some point, and then work on different branch to compare, develop new feature, deal with another topic and so on. You don't need to fork a new repo or copy the repo to do this but just "branch". Different branch will not influence each other but only share the same starting point. Finally you can "merge" different branch just like you merge two forked repos or you can leave the branch forever, and "checkout" to any branch you want develope on. Find the branch function in the github and try create new branch, "checkout"(switch) to it and "commit". Merge branch
- [ ] How you want to revert commit or any other operation? This is not trivial. The simplest way is to be really careful before commit! We will discuss this in a special chapter. 

## Local git operation
OK. If you finish all the thing below, you are already familiar with all the git operation despite you perform this on the github website. Next we will just translate the click on website to some commands in the terminal. The only two differences are that you now have some special git commands to download and upload the repo from/to github, and you have to deal with so called "stage". 

When working locally, use git status whenever you feel not clear!

The useful download/upload commands are:
- git clone
- git fetch
- git checkout
- git push

The "stage" is a special concept when you use git in the local. After "clone", you have all the files in the local. But all your changes on the files are not considered before you add them set them to the "stage" status by git add xxx. remove the "stage" status by git reset HEAD -- xxx. And to recover all the changed files to the state you download from remote, use git checkout -- xxx, this will discard all the change locally before you really commit it. And remember use git rm when you want to delete something not directly rm them.



The advantage you use git in the local is that you can edit the file with your favorite editor and importantly, compile and test the codes.

Then next we will just use one exmaple to show how we do the same thing as previous chapter in local:

```

```
## How to undo or revert change?
One special comment on revert and undo the change in git.

It is safe to revert the commit one by one from the latest by  
- git revert commitid. 
- git commit --amend. In local, you can use this to re-edit just the previous commit, if you havn't upload(push) it.

But if you want to revert a huge amount of commits, what you really need may be to move the "HEAD" of one branch to one specific commit location by 
- git branch -f branchname commitid
   
   
### Create your own repo

### Other stuffs...
