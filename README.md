# Linux-Shell
#tutorials
http://www.learnshell.org/ learnshell<br>
https://www.shellscript.sh/ shellscript<br>
http://www.kancloud.cn/digest/linux-world/145277 linux基础与shell编程<br>
https://tinylab.gitbooks.io/shellbook/content/   Shell 编程范例<br>
https://autellinux.wordpress.com/2013/09/04/online-simulator-in-linux-practice-linux-commands/ shell大全<br>
#tool
https://www.shellcheck.net/  shell check<br>
https://www.tutorialspoint.com/execute_bash_online.php  shell online<br>
#video
http://study.163.com/course/introduction/838003.htm#/courseDetail [云知梦]Shell脚本编程<br>
http://study.163.com/course/introduction/1238027.htm#/courseDetail 10天学会Shell编程<br>
http://www.lthack.com/forum.php?mod=viewthread&tid=3757  尚观Shell视频教程<br>
http://www.imooc.com/learn/181  Linux Guide for Developers(happypeter)<br>


Java开发必会的Linux命令
1.查找文件

find / -name filename.txt 根据名称查找/目录下的filename.txt文件。

find . -name "*.xml" 递归查找所有的xml文件

find . -name "*.xml" |xargs grep "hello world" 递归查找所有文件内容中包含hello world的xml文件

grep -H 'spring' *.xml 查找所以有的包含spring的xml文件

find ./ -size 0 | xargs rm -f & 删除文件大小为零的文件

ls -l | grep '.jar' 查找当前目录中的所有jar文件

grep 'test' d* 显示所有以d开头的文件中包含test的行。

grep 'test' aa bb cc 显示在aa，bb，cc文件中匹配test的行。

grep '[a-z]\{5\}' aa 显示所有包含每个字符串至少有5个连续小写字符的字符串的行。

2.查看一个程序是否运行

ps –ef|grep tomcat 查看所有有关tomcat的进程

ps -ef|grep --color java 高亮要查询的关键字

3.终止线程

kill -9 19979 终止线程号位19979的进程

4.查看文件，包含隐藏文件

ls -al

5.当前工作目录

pwd

6.复制文件

cp source dest 复制文件

cp -r sourceFolder targetFolder 递归复制整个文件夹

scp sourecFile romoteUserName@remoteIp:remoteAddr 远程拷贝

7.创建目录

mkdir newfolder

8.删除目录

rmdir deleteEmptyFolder 删除空目录 rm -rf deleteFile 递归删除目录中所有内容

9.移动文件

mv /temp/movefile /targetFolder

10.重命令

mv oldNameFile newNameFile

11.切换用户

su -username

12.修改文件权限

chmod 777 file.java //file.java的权限-rwxrwxrwx，r表示读、w表示写、x表示可执行

13.压缩文件

tar -czf test.tar.gz /test1 /test2

14.列出压缩文件列表

tar -tzf test.tar.gz

15.解压文件

tar -xvzf test.tar.gz

16.查看文件头10行

head -n 10 example.txt

17.查看文件尾10行

tail -n 10 example.txt

18.查看日志类型文件

tail -f exmaple.log //这个命令会自动显示新增内容，屏幕只显示10行内容的（可设置）。

19.使用超级管理员身份执行命令

sudo rm a.txt 使用管理员身份删除文件

20.查看端口占用情况

netstat -tln | grep 8080 查看端口8080的使用情况

21.查看端口属于哪个程序

lsof -i :8080

22.查看进程

ps aux|grep java 查看java进程

ps aux 查看所有进程

23.以树状图列出目录的内容

tree a

ps:Mac下使用tree命令

24. 文件下载

wget http://file.tgz mac下安装wget命令

curl http://file.tgz

25. 网络检测

ping www.just-ping.com

26.远程登录

ssh userName@ip

27.打印信息

echo $JAVA_HOME 打印java home环境变量的值

28.java 常用命令

java javac jps ,jstat ,jmap, jstack

29.其他命令

svn git maven

28.linux命令学习网站:
https://explainshell.com/
