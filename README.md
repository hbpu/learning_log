# learning_log————基于python的学习笔记系统的学习与实现
## 版本控制
### 0.1 .gitignore
> 1. 安装一个名为“.ignore”的插件
根目录新建.gitignore文件,在要忽略版本控制的文件或目录，右键选择“add to .gitignore",但是.gitignore只能忽略原来没有commit的文件。
```markdown
如果已经commit,首先将本地缓存删除，然后重新添加，最后再commit，并且更新.gitignore文件。需要(注意加.)
- git rm -r --cached .
- git add .
- git commit -m "add 忽略配置文件上传"

## 项目初始化
### 0.1 Django环境项目配置
```python
1. 创建python的虚拟环境、解释器、包
- $ python -m venv ll_env
2. 激活虚拟环境
- $ ll_env\Script\activate
# 停止环境
- $ deactivate
3. 创建项目
- $ django-admin startproject learning_log .
4. 迁移数据库
- $ python manage.py migrate
5. 运行项目
- $ python manage.py runserver
6. 创建app
- $ python manage.py startapp learning_logs
7. 修改model中的数据后更新数据库
- $ python manage.py makemigrations learning_logs
- $ python manage.py migrate
8. 创建超级用户admin
- $ python manage.py createsuperuser