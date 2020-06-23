# VS Code

## SFTP 套件

**設定檔案**

> .vscode/sftp.json

```json
{
    "name": "My Server",
    "host": "kjhost",
    "protocol": "sftp",
    "port": 22,
    "username": "kj",
    "remotePath": "/home/kj/",
    "privateKeyPath": "/Users/kejyun/.ssh/id_rsa",
    "watcher": {
        "files": "**/*{bundle.css,bundle.css.map,bundle.js,bundle.js.map}",
        "autoUpload": true,
        "uploadOnSave": true,
        "autoDelete": false
    },
    "uploadOnSave": true
}
```

## 參考資料
* [SFTP - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=liximomo.sftp)
* [GitHub - liximomo/vscode-sftp: Super fast sftp/ftp extension for VS Code](https://github.com/liximomo/vscode-sftp)
* [透過 VSCode SFTP/SSH 自動同步 Server 程式碼 - Soul & Shell Blog](https://blog.toright.com/posts/6456/vscode-sftp-ssh-code-sync.html)
* [How does watcher works? · Issue #78 · liximomo/vscode-sftp · GitHub](https://github.com/liximomo/vscode-sftp/issues/78)
