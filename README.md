# learngit
git初学者
>本地对仓库文件的修改(删除)会出现上传错误问题
--------
目前解决方法是删除.git文件夹里的.COMMIT_EDITMSG.swp文件即可重新上传也可以直接在运行"git rm .git/.COMMIT_EDITMSG.swp"
