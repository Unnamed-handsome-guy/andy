### Git

#### 1.配置用户名

- git config --global user.name "github用户名"

#### 2.配置邮箱

- git config --global user.email "435142285@qq.com"

#### 3.创建一个目录

#### 4.cd进入该目录

#### 5.使用git init变成git可管理的仓库

#### 6.文件提交到仓库

- git  add  sunck.txt
- git commit -m "注释信息"

#### 7.命令

- git status 查看当前状态
- git log 查看提交过的日志
  - git log --pretty=oneline 查看提交的样式
- git reset --hard HEAD^ 回退上个版本
- git reset --hard HEAD~100 回退上100个版本
- git reset --hard HEAD  具体版本号  
- git checkout -- sunck.txt   回退(相当于撤销，回到最后一次git commit或者git add)

#### 8.创建SSH Key

- ssh-keygen -t rsa -C "Github邮箱"  获取公私钥

- 记录.shh目录位置

  ![](C:\Users\Administrator\Desktop\andy\img\ssh.png)

- 复制公钥在GitHub添加ssh key

![](C:\Users\Administrator\Desktop\andy\img\GitHub.png)

- 输入 ssh -T git@github.com  (确认)

![](C:\Users\Administrator\Desktop\andy\img\ssh1.png)

#### 9.在GitHub创建远程仓库

#### 10.关联远程仓库

- git remote add origin 远程仓库地址（https://github.com/Unnamed-handsome-guy/andy.git）

- git remote rm origin 删除关联

#### 11.推送本地库到远程库（需要先把远程库拉到本地）

1. 远程库拉到本地库
   - git pull origin master![](C:\Users\Administrator\Desktop\andy\img\pull.png)
2. 推送本地库到远程
   - git push origin master
3. 创建.gitignore文件
   - 该文件下的名字不会被上传到github上

#### 12. 远程克隆

- git clone https://github.com/Unnamed-handsome-guy/andy.git

#### 13.分支

1. 创建分支
   - ​	git branch 分支名
2. 切换分支
   - ​	git checkout 分支名
3. 创建切换分支
   - git checkout -b 分支名