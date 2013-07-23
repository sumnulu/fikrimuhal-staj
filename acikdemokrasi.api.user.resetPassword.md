# Açıkdemokrasi API Doc - user.resetPassword

[Back to API docs home](Home)

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/resetPassword' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, /' --data-binary '{"email":"test@example.com"}'

|

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
