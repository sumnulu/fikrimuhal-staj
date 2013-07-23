# Açıkdemokrasi API Doc - user.changeEmail

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be loggedin user or an administrator
- Loggedin user should always provide their password

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/1/changeEmail' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, /' --data-binary '{"email":"test@example.com","currentPassword":"myPassword"}'

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
  "status":"Error",
  "message":"Wrong password",
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