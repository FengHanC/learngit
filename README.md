# learngit

***

git学习指南（笔记）

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

# 本地对仓库文件的修改(删除)会出现上传错误问题
  * 目前解决方法是删除.git文件夹里的.COMMIT_EDITMSG.swp文件即可重新上传
  * 也可以直接在运行"git rm .git/.COMMIT_EDITMSG.swp"
