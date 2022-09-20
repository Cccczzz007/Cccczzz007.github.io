# 永久禁止自动更新的步骤

## **步骤 1:** 按下键盘 Windows + X，选择 「Windows PowerShell (管理员)」。

![1](https://cdn.jsdelivr.net/gh/Cccczzz007/pic@main/pictures/1.png)

## **步骤 2:** 弹出的界面中输入 `sc.exe config wuauserv start= disabled` 后按回车，其用途是禁止 Windows 启动更新服务。

![![img](..图像1-16487307602672.png)](https://cdn.jsdelivr.net/gh/Cccczzz007/pic@main/pictures/![img](..图像1-16487307602672.png).png)





## **步骤 3:** 继续输入 `sc.exe stop wuauserv` 后按回车，其用途是停止当前正在运行的 Windows 更新服务。



![![img](..图像1-16487307724554.png)](https://cdn.jsdelivr.net/gh/Cccczzz007/pic@main/pictures/![img](..图像1-16487307724554.png).png)



步骤完成，你以后再也不会见到 Windows 10 自动更新了。若你想验证一下，可以前往 Windows 10 的更新界面，此刻会看到提示「遇到错误：更新服务无法正常运行」。

**注：本方法仅适用于终止未来可能有的更新，无法阻止已进入待安装状态的更新。**



# 恢复自动更新

若你想恢复自动更新，只需输入 `sc.exe config wuauserv start= auto` 即可。



# 太长不看

`sc.exe config wuauserv start= disabled`



sc.exe config wuauserv start= disabled



恢复



`sc.exe config wuauserv start= auto`



sc.exe config wuauserv start= auto





