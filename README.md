# local-to-origin
本地项目推送到GitHub仓库

git init  
git add -A  
git commit -m "first commit"  
git remote add origin https://github.com/Panamer/project-name.git  
git push -u origin master

如果仓库里有文件要先git pull 再 push

git pull 失败 ,提示：fatal: refusing to merge unrelated histories
关于这个问题，可以参考http://stackoverflow.com/questions/37937984/git-refusing-to-merge-unrelated-histories。

在进行git pull 时，添加一个可选项

git pull origin master --allow-unrelated-histories
