# 连接安卓设备
---
>不管通过哪种方式连接，都需要打开 `开发者模式`, 如下图

![](https://raw.githubusercontent.com/zhengaimin/obsidian-picbed/main/img/20231027011628.png)

---

- 通过 USB 连接
	直接执行 `adb advices` 即可
	显示效果入下（我自己的没有实现这种效果, 应该是和驱动有关）
	
	![image.png](https://raw.githubusercontent.com/zhengaimin/obsidian-picbed/main/img/20231027011504.png)

- 通过 WIFI 连接
	开启 <mark style="background: #FFB8EBA6;">无线调试</mark>
	输入命令 `adb connect 192.xxx.x.xx:40769` -> 运行结果
	![1698340526030.png](https://raw.githubusercontent.com/zhengaimin/obsidian-picbed/main/img/1698340526030.png)
	![image.png](https://raw.githubusercontent.com/zhengaimin/obsidian-picbed/main/img/20231027011606.png)

# ADB 命令
---
```Shell
# 用于列出当前连接到计算机的 Android 设备
adb devices

# adb 停止服务
adb kill-server
# adb 开启服务
adb start-server

# 端口映射
adb reverse tcp:8081 tcp:8081

# 沙盒
adb shell
# 查看目录
ls
# 退出沙盒
exit

# 通过 ip 地址远程连接设备
adb connect 192.xxx.x.xx:40769
# 通过 ip 地址断开设备
adb disconnect 192.xxx.x.xx:40769
```

