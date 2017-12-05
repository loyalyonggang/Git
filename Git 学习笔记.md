# Git 学习笔记

loyalyonggang	

2017年12月5日



## 本地上传到远程仓库

1. 建立项目,进入项目文件夹 

2. 初始化ssh key 参见官网指南.(本机生成一对key,public key传到官网sshkey下面)
   <https://help.github.com/articles/generating-ssh-keys/>

3. 初始化用户名,邮箱

   $ `git config --global user.name "loyalyonggang"`
   $ `git config --global user.email "loyalyonggang@gmail.com"`

4. `git init` git初始化

5. `git add . `添加当前文件夹的所有文件

6. `git commit -m "message for this commit" `提交

7. `touch README.md `建立程序说明文档   也可以直接用echo语句  `echo "machine-learning">>README.md  `

8. `git add README.md` 添加单个

9. `git status` 查看git状态

10. 去github网站建立一个repo 如"test.git"

11. `git remote add origin git@github.com:loyalyonggang/test.git`   远程添加
    如果遇到了fatal: remote origin already exists.输入:

    `git remote rm origin`

12. `git remote add origin git@github.com:loyalyonggang/test.git`

13. `git push -u origin master`  push到远程仓库，同时设置跟踪分支，下次push的时候，直接输入git push就醒了，系统会自动用本地master分支跟踪远程master分支

14. ok！



## 下载远程仓库

git clone +ssh 