# Açıkdemokrasi API Doc - user.resetPassword

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be loggedin user or an administrator
- Passwords should be the same

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/user/1/changePassword?password=newPassword&password2=newPassword](http://localhost.acikdemokrasi.org:8080/api/1/user/1/changePassword?password=newPassword&password2=newPassword)

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