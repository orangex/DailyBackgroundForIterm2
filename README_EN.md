# DailyBackgroundForIterm2
Set background with bing-daily-pic for Iterm2

[README-中文]()

### Usage
1. replace all the path、filename with your actual path or as you need
2. chmod a+x /xx/downloader.sh 
3. move the .plist to /Users/xxx/Library/LaunchAgents and load it like this
```
launchctl load -w /xx/xx.plist
```
and these cmds may help
```
launchctl load   xx.plist
launchctl unload xx.plist
launchctl start  xx.plist
launchctl stop   xx.plist
launchctl list
```
in which "start" let you immediately run the .sh to check whether it could work
4. **Iterm2**->**Preferences**->**Profiles**->**General**->**command**->**Send text at start** ,fill it with path of **startText.sh**

### Notes
- you shold install wget at global level or called root？ anyway ，not user level
- 
