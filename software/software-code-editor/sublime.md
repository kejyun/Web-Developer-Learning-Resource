# Sublime

## 使用 SFTP 即時上傳檔案

**安裝套件**

使用 Sublime Packages Controller 安裝 `Simple FTP Deploy` 套件

**設定 sftp-config.json**

在專案目錄下建立 `sftp-config.json` 檔案，並將此設定值填入到檔案中，並加入自己主機的相關設定

```json
{
    // The tab key will cycle through the settings when first created
    // Visit http://wbond.net/sublime_packages/sftp/settings for help

    // sftp, ftp or ftps
    "type": "sftp",

    "sync_down_on_open": true,
    "sync_same_age": true,

    // 主機網址
    "host": "server.kejyun.com",
    // 帳號
    "user": "username",
    // 密碼
    // "password": "password",
    // Port
    "port": "22222",
    // 是否在儲存檔案時立即上傳檔案
    "upload_on_save" : true,

    // 專案目錄對應遠端路徑
    "remote_path": "/home/kejyun/project/folder",
    //"file_permissions": "664",
    //"dir_permissions": "775",

    //"extra_list_connections": 0,

    "connect_timeout": 30,
    //"keepalive": 120,
    //"ftp_passive_mode": true,
    //"ftp_obey_passive_host": false,
    // SSH 金鑰
    "ssh_key_file": "~/.ssh/id_rsa",
    //"sftp_flags": ["-F", "/path/to/ssh_config"],

    //"preserve_modification_times": false,
    //"remote_time_offset_in_hours": 0,
    //"remote_encoding": "utf-8",
    //"remote_locale": "C",
    //"allow_config_upload": false,
}

```

## 參考資料
* [Simple FTP Deploy - Packages - Package Control](https://packagecontrol.io/packages/Simple%20FTP%20Deploy)
