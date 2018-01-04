将如下内容保存为bat文件执行即可，因为这个脚本中有中文，需要将文件保存为ANSI编码，否则执行的时候中文会显示乱码。

使用win+R 快捷键，运行notepad，使用记事本保存为ANSI编码。

```bat
@echo off
::set /p ip=请输入IP:
::set /p domain=请输入域名IP:
::set hosts="c:\WINDOWS\system32\drivers\etc\hosts"
::echo %ip% %domain% >> %hosts%
set hosts="c:\WINDOWS\system32\drivers\etc\hosts"

echo. >> %hosts%
echo 192.168.0.241 jfgit.bzw.cn >> %hosts%

::显示hosts文件中的内容
type %hosts%

echo.
echo.
echo git 服务器 访问地址：http://jfgit.bzw.cn
echo.
pause

```



