# learning_log
版本控制 
0.1 .gitignore
> 1. 安装一个名为“.ignore”的插件
> 根目录新建.gitignore文件
> 在要忽略版本控制的文件或目录，右键选择“add to .gitignore"
> 但是.gitignore只能忽略原来没有commit的文件.
> 如果已经commit,需要(注意加.)：
> git rm -r --cached .
> git add .
> git commit -m "add 忽略配置文件上传"
> 首先将本地缓存删除，然后重新添加，最后再commit，并且更新.gitignore文件。
