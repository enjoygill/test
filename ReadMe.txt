1.git核心上传配置文件在.ssh文件中C:\Users\Administrator\.ssh
2.第一步在此文件夹即你建立的仓库中，点击右键git bash ，然后Git init,
接着利用ssh -T git@github.com 测试是否能链接github成功
如果是第一次就需要配置git，让git服务器知道你；
 （1）配置本地ssh key
$ ssh-keygen -t rsa -C "1873247496@qq.com" github上注册的邮箱
 （2）把本地生成的key复制到github官方网站ssh key中
再次验证ssh -T git@github.com 测试是否能链接github成功
3.注意如果你建立新仓库时候，必须输入用户名和邮箱，让git知道你是谁
$ git config --global user.name "enjoygill"
$ git config --global user.email "1873247496@qq.com"


--------------------------------上面是第一次做法，如果不是第一次直接从4开始
4如果上述都已经做好，直接git remote add origin git@github.com:enjoygill（用户名）/仓库名（test）.git
5.每次准备上传时，先git pull下，否则会报错。同时,commit后注意git status查看状态
git add +提交内容（添加到缓存区）
git commit -m "message" 
git push origin master   （这两步才是真正的提交）

6、如果是colne本地的话，需要新建一个文件夹，启动gitbash，输入git init
在打入命令git clone git@github.com:enjoygill/项目名字.git （一般不好直接clone仓库的某个文件）  

7从远程服务器克隆一个一模一样的版本库到本地,复制的是整个版本库，叫做clone.
（clone是将一个库复制到你的本地，是一个本地从无到有的过程）
 从远程服务器获取到一个branch分支的更新到本地，并更新本地库，叫做pull.
（pull是指同步一个在你本地有版本的库内容更新的部分到你的本地库）
 git pull相当于是从远程获取最新版本并merge（合并）到本地     
 git pull = git fetch + git merge，git fetch更安全一些

8修改，你clone本地后要修改后，如果你要提交，必须先保存到暂存区，才能提交上去。
要先加入到 staging area 的改动才会被 git commit 提交。同一个文件也可以 add 多次。
不想add可以：
git commit -m 'msg' <file>
或者
git commit -m 'msg' -a