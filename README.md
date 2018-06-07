# learngit
git初学者
## git使用指南
- 链接远程仓库git remote add origin （仓库链接）
- git init 初始化（创建）仓库
- git add test.txt添加到仓库
- git commit -m "提交描述" 提交
```
$ 列1
$ 列2
```
--------------------
>本地对仓库文件的修改(删除)会出现上传错误问题
--------
目前解决方法是删除.git文件夹里的.COMMIT_EDITMSG.swp文件即可重新上传也可以直接在运行"git rm .git/.COMMIT_EDITMSG.swp"
