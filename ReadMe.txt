1.git核心上传配置文件在.ssh文件中C:\Users\Administrator\.ssh
2.第一步在此文件夹即你建立的仓库中，点击右键git bash ，然后Git init,
接着利用ssh -T git@github.com 测试是否能链接github成功
3.注意如果你建立新仓库时候，必须输入用户名和邮箱，让git知道你是谁
4.每次准备上传时，先git pull下，否则会报错，然后,commit后注意git status查看状态
git add .
git commit -m "message"
git push origin master