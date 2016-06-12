# fetch使用

#### fetch是新一代的网络请求方式

```
   return fetch('/getSelfInfo',/*请求地址 默认GET*/ {
        method: 'POST',
        headers: {
            'Accept': 'application/json, text/javascript, */*; q=0.01', //接受数据格式
            'Content-Type': 'application/json; charset=UTF-8', //请求数据格式
        },
        credentials: 'include'//使用cookie  默认不使用cookie,
        body: JSON.stringify({user: 'xxx'})
    }).then(function (data) {
                data.json().then(function(json){
                    console.log(json)
                })
            };

```
