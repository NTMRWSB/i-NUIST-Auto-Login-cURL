# i-NUIST-Auto-Login-cURL
群晖狂喜

''
curl 'http://a.nuist.edu.cn/api/v1/login' \
  -H 'Accept: application/json, text/plain, */*' \
  -H 'Accept-Language: zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6' \
  -H 'Connection: keep-alive' \
  -H 'Content-Type: application/json;charset=UTF-8' \
  -H 'DNT: 1' \
  -H 'Origin: http://a.nuist.edu.cn' \
  -H 'Referer: http://a.nuist.edu.cn/authentication' \
  -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36 Edg/105.0.1343.27' \
  --data-raw '{"username":"02502375845","password":"513090","channel":"4","ifautologin":"0","pagesign":"secondauth","usripadd":"10.12.240.123"}' \
  --compressed \
  --insecure
  ''
