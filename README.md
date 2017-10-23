# GitTest
用过SVN，学一下Git

```
$ ssh-keygen -t rsa -C "Github账号"   #生成ssh秘钥
```
1. 后面会提示输入存放路径以及文件名（/d/github/key），然后密码设置
2. 到Github上把刚生成的key.pub

记一下部分常用命令
```
$ git init                                # 初始化本地仓库
$ git add README.md                       # 添加文档文件到暂存区
$ git rm README.md                        # 删除文件
$ git commit -m "添加 README.md 文件"      # 提交暂存区的文件及备注到当前分支

$ git remote add origin git@github.com:0Kelvins/GitTest.git #添加远程仓库源
$ git push -u origin master #推送到远程仓库

$ git clone https://github.com/0Kelvins/GitTest.git #克隆远程仓库到当前目录下

$ git checkout -- file #用版本库里的版本替换工作区的版本
$ git reset HEAD file  #可以把暂存区的修改撤销掉（unstage），重新放回工作区
$ git add --all                       # 添加当前目录所有文档文件到暂存区
```
1. 克隆仓库不需要先建本地仓库，仓库源添加一次就可以了，克隆的不需要添加
2. 源仓库地址可以有两种，SSH地址``git@github.com:0Kelvins/GitTest.git``，URL地址``https://github.com/0Kelvins/GitTest.git``都可以

顺便记录一下下面几个命令
```
$ cd . > test.txt          #在当前目录新建文件test.txt

$ echo "内容" > test.txt
$ echo "内容" >> test.txt  #写入内容到文件

$ cat test.txt             #查看文件内容
$ rm test.txt              #删除文件
```


