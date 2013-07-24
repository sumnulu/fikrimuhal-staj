# Açıkdemokrasi API Doc - user.checkEmailAddress

[Back to API docs home](Home)

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/checkEmailAddress
- Content-Type: application/json
- Raw-body (data-binary): {"email":"test@example.com"}

```
{
  "status": "OK",
  "data": {
    "available": true,
    "email": "user@example.com"
  }
}
```