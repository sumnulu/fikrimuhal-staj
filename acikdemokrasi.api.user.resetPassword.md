# Açıkdemokrasi API Doc - user.resetPassword

[Back to API docs home](Home)

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/user/resetPassword?email=test@example.com](http://localhost.acikdemokrasi.org:8080/api/1/user/resetPassword?email=test@example.com)

```
{
  "status":"Error",
  "message":"Object not found",
  "code":620,
  "data": []
}
```
```
{
  "status":"OK",
  "message":"Password reset information has been sent to your address"
}
```
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