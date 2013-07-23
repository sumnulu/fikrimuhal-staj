# Açıkdemokrasi API Doc - user.resetPasswordWithToken

[Back to API docs home](Home)

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/resetPasswordWithToken' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, /' --data-binary '{"token":"3e815c58-946f-4d6b-989b-3dd20be59303","newPassword":"123","newPassword2":"123"}'

|

```
{
  "status":"Error",
  "message":"Invalid Token",
  "code":999
  "data": []
}
```
```
{
  "status":"Error",
  "message":"Passwords are not same",
  "code":999
  "data": []
}
```
```
{
  "status":"OK",
  "message":"Your password has been changed"
}
```
