# Learning Git

#### 配置环境
1. `git config --global user.name "mingfeii"`
2. `git config --global user.email "mingfeii@outlook.com"`
3. `git init	`	
4. `ssh-keygen -t rsa -C "mingfeii@outlook.com"`,一路默认
5. 登陆GitHub，打开“Account settings”，“SSH Keys”页面，然后，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容

![ssh0](https://raw.githubusercontent.com/mingfeii/tutorial-note/master/ssh0.png) 
![ssh1](https://raw.githubusercontent.com/mingfeii/tutorial-note/master/ssh1.png) 

#### 提交
1. 在github上先建立一个repo,比如`toturial-note`
2. 克隆到本地`git clone git@github.com:mingfeii/tutorial-note.git`
3. `git remote add origin git@github.com:mingfeii/tutorial-note.git`
4. `git add file`
5. `git commit -m "msg' file `
6. `git push  origin master` or `git push  -u origin master`

#### 版本控制
* `git status` 查看提交状态
* `git difff `
* `git log` 命令显示从最近到最远的提交日志
* `git`的commit id不是1，2，3……递增的数字，而是一个SHA1计算出来的一个非常大的数字，用十六进制表示
* `git`中，用HEAD表示当前版本，也就是最新的提交,上一个版本就是HEAD^
* `git reset ` 回退，`git reset --hard HEAD^` 回退上一个版本，`git reset --hard 1094a` 版本号不用写全
* `git checkout -- readme.txt`意思就是，把readme.txt文件在工作区的修改全部撤销,就是让这个文件回到最近一次git commit或git add时的状态
* `git rm`删除文件，并且`git commit`