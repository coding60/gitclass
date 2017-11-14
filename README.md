win7下安装git及关联使用github
--by coding60.com qq: 761593965
一，软件安装环境：
  Operating System: Windows 7 旗舰版 64-bit (6.1, Build 7601) Service Pack 1 (7601.win7sp1_ldr.170913-0600)
  Language: Chinese (Simplified) (Regional Setting: Chinese (Simplified))
System Manufacturer: Hewlett-Packard
 System Model: HP 431 Notebook PC              
 BIOS: InsydeH2O Version 03.60.50F.22
 Processor: Intel(R) Core(TM) i3-2330M CPU @ 2.20GHz (4 CPUs), ~2.2GHz
 Memory: 4096MB RAM
二、软件版本
1. Git-2.14.3-64-bit
三、软件下载
1. Git-2.14.3-64-bit：
2. Git中文参考手册CHM：
3.如不能下载请联系QQ ：761593965
四、安装过程：
1.安装git.
2.注册github账户，网址是. github.com，特别提醒一定要用Google Chrome浏览器，不然配置SSH Keys会找不到界面。
3. 配置Git, 首先在本地创建ssh key,打开gitbash,
输入： ssh-keygen -t rsa -C "your_email@youremail.com"
这里输入你在github上注册的邮箱。之后会要求确认路径和输入密码，我们这使用默认的一路回车就行。成功的话会在git安装目录/下生成.ssh文件夹，进去，打开id_rsa.pub，复制里面的key。
4.配置github上的SSH Keys，进入github，进入 Account Settings（账户配置），左边选择SSH Keys，Add SSH Key,title随便填，粘贴在你电脑上生成的key。

5.验证是否成功，在git bash下输入：ssh -T git@github.com.
如果是第一次的会提示是否continue，输入yes就会看到：You've successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。
6.在github上创建一个项目，进入github，在Repositories页面右侧有一个New按钮，点击它来创建新的项目代码库。
7.将github上创建的项目克隆到本地，打开gitbash,
切换到你本地的项目目录，我的在d:git/
输入：cd d:
输入：cd git
输入：git clone username@host:/path/to/repository
其中username@host:/path/to/repository是指的githubh 上项目地址，进入项目后，点击cloneordonwload可以获得。
8.将本地项目文件上传到到github, 在git bash下输入:
git add test.txt //添加test.txt 
git commit -m “push test.txt”  //提交描述
git push origin master //将代码提交到远程服务器，这个就是描述



视频教程及软件下载地址：

60编程网

http://d.coding60.com
 

