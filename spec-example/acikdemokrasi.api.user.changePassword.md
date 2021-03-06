# Açıkdemokrasi API Doc - user.changePassword

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be loggedin user or an administrator
- Password should be at least 6 characters

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/1/changePassword
- Content-Type: application/json
- Raw-body (data-binary): {"password":"newPassword"}

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
  "status":"Error",
  "message":"Passwords are not the same",
  "code":999,
  "data": []
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