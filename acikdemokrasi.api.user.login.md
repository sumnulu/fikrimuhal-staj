# Açıkdemokrasi API Doc - user.login

[Back to API docs home](Home)

### Requirements
- User should not be logged in
- Username and password should be valid
- authType should be "rememberMe" or "plain"
- Email address should be verified

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/login?authType=plain
- Content-Type: application/json
- Raw-body (data-binary): {"email":"test@example.com","currentPassword":"password"}

---

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/login?authType=rememberMe

```
{
  status:"Error",
  message:"You are already logged in",
  code: 620,
  data: []
}
```
```
{
  status:"Error",
  message:"Email address or password cannot be blank",
  code: 611,
  data: []
}
```
```
{
  status:"Error",
  message:"Object not found",
  code: 620,
  data: []
}
```
```
{
  "status":"OK",
  "data": {
    "facebook": [
      "id":1
    ]
    "id":999,
    "firstName":"first",
    "middleName":"middle",
    "lastName":"last",
    "email":"user@example.com",
    "fullName":"first middle last",
    "pictureUrl":"",
    "type":"Vatandaş",
    "totalVotes":24,
    "totalTopics":4,
    "isAdmin":1
  }
}
```