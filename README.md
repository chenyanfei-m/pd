# pd

网络无法连接问题:
前往 /Library/Preferences/Parallels 目录（在访达的菜单栏中点击“前往->前往文件夹”）。
打开network.desktop.xml文件。
搜索 UseKextless
找到
<UseKextless>-1</UseKextless>
或
<UseKextless>1</UseKextless>
修改为
<UseKextless>0</UseKextless>
如果我们搜索不到这个标签，那么就在根标签下创建它，如下图
点击保存，输入开机密码。
Parallels Desktop 16 big sur 下无法联网和无法使用usb的解决办法

USB无法识别问题:
前往/Library/Preferences/Parallels文件夹。
打开 dispatcher.desktop.xml 文件。
找到 
<Usb>0</Usb>
修改为
<Usb>1</Usb>
修改后，重启 Parallels Desktop以及windows，即完美解决以上问题。

