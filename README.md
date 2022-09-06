# i-NUIST-Auto-Login-cURL  
## 群晖用户狂喜  
### 使用指南：  
1. 登录DSM->控制面板->计划任务  
2. 选择新增用户定义的脚本，无需使用root账户，将以下代码修改后粘贴进去  
```
curl 'http://a.nuist.edu.cn/api/v1/login' \
  -H 'Accept: application/json, text/plain, */*' \
  -H 'Accept-Language: zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6' \
  -H 'Connection: keep-alive' \
  -H 'Content-Type: application/json;charset=UTF-8' \
  -H 'DNT: 1' \
  -H 'Origin: http://a.nuist.edu.cn' \
  -H 'Referer: http://a.nuist.edu.cn/authentication' \
  -H 'User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36 Edg/105.0.1343.27' \
  --data-raw '{"username":"114514","password":"1919","channel":"4","ifautologin":"0","pagesign":"secondauth","usripadd":"10.12.240.123"}' \
  --compressed \
  --insecure
  ```  
### Tips：  
1. "username":"114514"中，填写自己的上网账号  
2. "password":"1919"中，填写自己的上网账号密码  
3. "channel":"4"代表运营商，其中4为中国联通  

| 代码 | 运营商   |
|------|----------|
| 1    | CERNET   |
| 2    | 中国电信 |
| 3    | 中国移动 |
| 4    | 中国联通 |
