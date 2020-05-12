# testRepo
This is to learn some git tricks
1.clone your repo -> git clone https://github.com/saur0906/testRepo.git

2.change working dir to cloned repo -> cd testRepo/

3.check the existing remote for your repo - git remote -v

4.check all the branches for your repository - git branch -a

5.now fetch the remote repos - git fetch

6.now checkout the remote directory to your local by - git checkout origin/dev

7.check the current branch - git branch -a

8.add a file to your local checked out branch - eg.test1.json

9.check the status with - git status
result should be like below 
HEAD detached at origin/dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	test1.json

nothing added to commit but untracked files present (use "git add" to track)


10.Add the untracked files - git add --all
EAD detached at origin/dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   test1.json


11.Now commit to your local repo -
haabil9692@jehennum:~/git_repos/play_again/testRepo$ git commit -m "test.json added"
[detached HEAD 988147a] test.json added
 1 file changed, 3 insertions(+)
 create mode 100644 test1.json
haabil9692@jehennum:~/git_repos/play_again/testRepo$ git status
HEAD detached from origin/dev
nothing to commit, working directory clean

12.haabil9692@jehennum:~/git_repos/play_again/testRepo$ git push -u origin HEAD:dev
Username for 'https://github.com': SAUR0906
Password for 'https://SAUR0906@github.com': 
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 300 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/saur0906/testRepo.git
   18deb5b..988147a  HEAD -> dev
