# Learning Git

#### 配置环境
1. `git config --global user.name "mingfeii"`
2. `git config --global user.email "mingfeii@outlook.com"`
3. `git init	`	
4. `ssh-keygen -t rsa -C "mingfeii@outlook.com"`,一路默认
5. 登陆GitHub，打开“Account settings”，“SSH Keys”页面，然后，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容
![ssh0](/home/s/tutorial-note/ssh0.png) 
![](/home/s/tutorial-note/ssh1.png) 
#### 提交
1. 在github上先建立一个repo,比如`toturial-note`
2. 克隆到本地`git clone git@github.com:mingfeii/tutorial-note.git`
2. `git add file`
3. `git commit -m "msg' file `


