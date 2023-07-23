# Vulnerability Description
I found a Reflected Cross-Site Scripting （XSS） in the latest version of Emby server version  4.7.13.0
official address：
https://emby.media/
https://github.com/MediaBrowser/Emby.Releases   

# Vulnerability Details

Everything after /web/ is reflected. See the attachments for an example: 
```
http://<ip>:<port>/web/%3Cimg%20sRc=l%20oNerrOr=alert('xss')%20x%3E
```


