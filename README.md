# learngit

***

git学习指南（笔记）
更多内容请移步wiki查看

## 创建SSH Key：
* $ ssh-keygen -t rsa -C “405029223@qq.com” 
* 回车三次生成 .ssh文件
* 登陆GitHub，打开“Account settings”，“SSH Keys”页面：然后，点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容
# 配置个人信息
1. $ git config --global user.name "FengHanC"
2. $ git config --global user.email "405029223@qq.com"
## git使用指南
* git init 初始化（创建）仓库

***

* git add 文件
* git commit -m "提交描述"
###  修改之后重新提交
提交必走流程：
1. git add .(文件添加跟踪)
2. git commit -m '提交描述' （给提交加描述，以后看日志会更清楚）
## 以上两边只有对文件有修改就要执行。

***

* git push -u origin master 这是提交到远程仓库操作
* git diff 查看文件修改信息

# 创建并切换分支
$ git checkout -b dev 

# 链接远程仓库的两种方法
1. * **链接远程仓库`git remote add origin git@github.com:FengHanC/learngit.git`** 
   * _（仓库链接格式：git@github.com:用户名/仓库名.git）_
2. * **在GitHub上创建并克隆仓库`git clone git@github.com:FengHanC/learngit.git`**
   * _（格式同上）这时本地就会有一个仓库了（cd：指定仓库存放位置）_

> ### 远程仓库修改会影响本地的提交
> * 这时就需要用到git pull（推送）来同步本地仓库
> * 这时就可以正常push了，注意：git add/git commit是不能省的

### 版本回退
* `git log` 查看提交日志（查看日志id）
* `git reset --hard id` 日志id（取一小段6-8个左右，git会自动补全）

## 常见错误
userA 提交了一个01.txt 文件
userB 也提交一个01.txt 文件造成冲突
解决方式：
1. 先拉取线上版本git pull
2. 如果
