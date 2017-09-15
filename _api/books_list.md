---
title: /projects 获取项目列表
position: 1
type: get
description: 获取企业下所有项目列表
right_code: >-
  ~~~ json[  {    "id": 1,    "title": "The Hunger Games",    "score": 4.5,   
  "dateAdded": "12/12/2013"  },  {    "id": 1,    "title": "The Hunger
  Games",    "score": 4.7,    "dateAdded": "15/12/2013"  },]~~~{:
  title="Response" }~~~ json{  "error": true,  "message": "Invalid offset"}~~~{:
  title="Error" }
---


<dl><dt>pageNo</dt><dd>分页参数，可选</dd><dd>页码从1开始，默认取值1</dd><dt>pageSize</dt><dd>每页包含记录数，可选</dd><dd>默认取值20</dd></dl>

该接口提供获取当前登陆企业下所有项目列表信息。

{: .info}

Lists all the photos you have access to. You can paginate by using the parameters listed above.

```javascript
$.get("http://api.myapp.com/books/", { "token": "YOUR_APP_KEY"}, function(data) {
  alert(data);
});
```

```python
r = requests.get("http://api.myapp.com/books/", token="YOUR_APP_KEY")
print r.text
```

```javascript
var request = require("request");
request("http://api.myapp.com/books?token=YOUR_APP_KEY", function (error, response, body) {
  if (!error && response.statusCode == 200) {
    console.log(body);
  }
});
```

```bash
curl http://sampleapi.readme.com/orders?key=YOUR_APP_KEY
```