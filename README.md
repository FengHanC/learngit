# learngit

git学习指南（笔记）

## git使用指南
- git init 初始化（创建）仓库
- git add test.txt添加到仓库
- git commit -m "提交描述" 这是内容提交到本地仓库
- git push -u origin master 这是提交到远程仓库操作


```sh

$ 链接远程仓库的两种方法
$ 链接远程仓库git remote add origin git@github.com:FengHanC/learngit.git 
（仓库链接格式：git@github.com:用户名/仓库名.git）;
$ 在GitHub上创建并克隆仓库
￥ git clone git@github.com:FengHanC/learngit.git
（格式同上）这时本地就会有一个仓库了（cd：指定仓库存放位置）
$ 远程仓库修改会影响本地的提交
$ 这时就需要用到git pull（推送）来同步本地仓库
$ 这时就可以正常push了，注意：git add/git commit是不能省的

```


--------

###本地对仓库文件的修改(删除)会出现上传错误问题
 目前解决方法是删除.git文件夹里的.COMMIT_EDITMSG.swp文件即可重新上传
 也可以直接在运行"git rm .git/.COMMIT_EDITMSG.swp"

--------
