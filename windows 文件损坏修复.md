## 错误码 80070490

日志出现类似 |E|audio_device_wasapi.cc:386|130C|AUDIO-WASAPI|GetDevice failed hr=80070490

hr=80070490 错误的关键在于 ​​ 系统地排查和修复受损的系统组件 ​​。建议你按照从简到繁的顺序尝试：​​ 先进行系统文件修复（SFC 和 DISM）​​，这通常能解决大部分问题；如果问题与更新相关，再尝试 ​​ 重置 Windows 更新组件 ​​；若错误出现在特定的驱动或软件安装场景，则可检查 ​​ 驱动程序队列和磁盘空间 ​​

使用 CMD 用管理员执行

```shell
# ​​立即扫描所有受保护的系统文件，并尝试修复发现的问题​​。这是最常用也是功能最全面的命令
sfc /scannow
```

## 错误码 0

xx:xx:xx.xxx|E|audio_device_wasapi.cc:1193|5A5C|AUDIO-WASAPI|device is not ACTIVE hr=0 state=0x00000008

重新插拔设备，恢复不了的话，重装驱动
