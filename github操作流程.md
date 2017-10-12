配置git：
    
    输入命令：git config --global user.name "你的用户名"
    输入命令：git config --global user.email 你的邮箱地址

添加托管文件：    
    
    输入命令：git add ./
    
commit项目：
    
    输入命令：git commit -m "描述信息"
    
上传项目：
    
    输入命令：git remote add origin 仓库地址
    输入命令：git push -u origin master
    输入命令：git pull
    输入命令：git push 

git常用命令：

1、git clone 仓库地址  //克隆仓库代码到本地

2、git diff  //查看本地代码与远程代码有哪些不同

3、git pull //从远程拿到最新版本代码（提交代码时，忌讳直接提交。每次提交代码之前，一定要保证本地的代码是最新的，即先执行git pull）

4、git branch //查看本地代码属于仓库的哪个分支

5、git branch -a //查看仓库都有哪些分支

6、git checkout 分支名 //切换分支（注：不建议使用，最好给一个分支单独建立一个文件夹）

7、git clone -b 分支名 仓库地址 //克隆指定分支的仓库代码到本地

8、git push -u origin 分支名（分支名通常为master）

四、git常见问题： 

git pull失败问题：有时候git pull会出现失败的情况，即本地代码和远程代码出现冲突，这种情况需要手动解决。

解决冲突方法：

1、git stash //将本地文件回馈上一步操作

2、git pull   //将新代码下载下来

3、git stash pop //会将已经冲突的文件合并，代码中会出现 “<<<<<” 和 “>>>>>”的符号，符号之间的代码就是本地和远程的冲突的部分，协商去解决。

4、解决好后再git pull，git commit，git push