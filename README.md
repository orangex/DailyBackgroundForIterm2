# DailyBackgroundForIterm2

Set background with bing-daily-pic for Iterm2

## [README-EN](https://github.com/orangex/DailyBackgroundForIterm2/blob/master/README_EN.md)

### 使用

1. 把文件名和文件内的路径根据你的需要全部替换成你的实际路径
2. chmod a+x /xx/downloader.sh
3. 把 .plist 移动到 /Users/xxx/Library/LaunchAgents 然后像下面这样 load 到 plist 中

```
launchctl load -w /xx/xx.plist
```

  还有一些 launchctl 的命令

```
launchctl load   xx.plist
launchctl unload xx.plist
launchctl start  xx.plist
launchctl stop   xx.plist
launchctl list
```

  "start" 是立即运行 .plist 中配置的脚本而忽视设定的时间，可以拿来检查你的 downloader.sh 有没有问题

1. **Iterm2**->**Preferences**->**Profiles**->**General**->**command**->**Send text at start** ,在这里填入 **startText.sh** 的路径

### 注意

- downloader 中需要的 wget 你可能需要去安装，并且安装到 root 这个级别还是叫做全局，反正不是 user 级别。
- .plist 发生改变后需要 unload  一下，再 load
- 小细节可以 google



最后的效果长这样

![](https://ws2.sinaimg.cn/large/006tKfTcgy1fjqzdtf2mxj31kw0yjaqt.jpg)