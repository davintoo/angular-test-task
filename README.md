# angular-test-task

1) Register and activate user on https://sandbox.davintoo.com/
2) Create Angualr(version >= 10.x) appliaction. 
Application should authorize by login/password
```
curl -X POST 'https://sandbox.davintoo.com/api/rest.php/auth/session' -H 'Content-Type: application/json;charset=UTF-8' --data-binary '{"email":"youremail","password":"yourpassword"}'
```
and fetch resources from Knoweladge Base
https://sandbox.davintoo.com/knowledge-base/search
use API call
```
curl 'https://sandbox.davintoo.com/api/rest.php/knowledge-objects?page=1&count=10&filter[type]=knowledge_base&action=search'  -H 'Content-Type: application/json;charset=UTF-8' -H 'Authorization: Bearer Your_JWT_TOKEN_HERE'
```
show found resources in list.

![Mockup](https://raw.githubusercontent.com/davintoo/angualr-test-task/master/Angular%20Task.jpg)
