# CORS(Cross-Origin Resource Sharing)


將您要測試遠端 API 的服務網址加入下方的 `http://EXAMPLE.COM/SOME/API` 位置，就可以至抓取到 API 的允許連線來源是什麼

```shell
curl -I -X OPTIONS \
  -H "Origin: http://EXAMPLE.COM" \
  -H 'Access-Control-Request-Method: GET' \
  http://EXAMPLE.COM/SOME/API 2>&1 | grep 'Access-Control-Allow-Origin'
```

假如 API 有設定 `Access-Control-Allow-Origin` 的話則會顯示下方訊息，如果都沒有設定的話，就會顯示空白

```shell
Access-Control-Allow-Origin: *
```

# 參考資料
* [Test CORS with cURL · GitHub](https://gist.github.com/exAspArk/07bbbafa2a9171b6c260989780cc0955)
