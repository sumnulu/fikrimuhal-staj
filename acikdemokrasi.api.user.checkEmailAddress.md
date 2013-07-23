# Açıkdemokrasi API Doc - user.checkEmailAddress

[Back to API docs home](Home)

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/checkEmailAddress' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, /' --data-binary '{"email":"test@example.com"}'

|

```
{
  "status": "OK",
  "data": {
    "available": true,
    "email": "user@example.com"
  }
}
```