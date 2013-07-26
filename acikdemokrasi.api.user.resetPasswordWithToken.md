# Açıkdemokrasi API Doc - user.resetPasswordWithToken

[Back to API docs home](Home)

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/changePasswordWithToken
- Content-Type: application/json
- Raw-body (data-binary): {"token":"2313-23123-213213","password":"newPassword"}

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
  "status":"OK",
  "message":"Your password has been changed"
}
```
