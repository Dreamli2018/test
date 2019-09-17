Git 的使用

1:建立远程连接，ssh

2:创建本地仓库，初始化本地仓库，git init；

3：添加项目到本地仓库，git add . ;

4: 提交， git commit -a -m "添加注释"

5: 和对应远程github仓库建立连接，git remote add origin "对应远程仓库的地址"

6：把本地仓库的项目推送到远程仓库，git push -u origin master ；"如果是第一次提交项目"

7:对项目进行了修改之后，git commit -a -m "添加注释"；

8: 再次推送，此时不需要重新和远程仓库再建立连接了，因为之前已经连接过了，直接 git push 就可以了；

9: 创建分支以及合并分支，git checkout -b iss01命令，一步操作即可将分支创建好并检出到对应的分支iss01上；或者分两步也可以，即先创建分支，git branch iss01，然后再检出到分支iss01，git checkout iss01；对对应的内容进行修改，vim 对应文件名，例如 vim index.html;  "i"命令可以插入，esc键退出，：后跟wq退出并保存修改，

10:修改完毕进行提交，git commit -a -m "添加注释"，

11:合并分支，先切回到master，git checkout master，然后git merge branch iss01 即将分支iss01的内容合并到master上了，

12:如果分支不需要了，可以删除分支，git branch -d iss01 即将分支iss01删除，不可以在当前分支对当前分支进行删除，必须切换到master或者其他分支上才可以

13:git解决合并冲突，合并遇到冲突时，可以手动删除不需要的部分，然后再次git add . 之后git就会默认冲突已经解决然后再commit就OK了，或者使用git mergetool来解决冲突



