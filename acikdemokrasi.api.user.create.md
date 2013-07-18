# Açıkdemokrasi API Doc - user.create

[Back to API docs home](Home)

### Requirements
- User should be logged in
- Email field cannot be empty or existing

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/user/create?firstName=first&middleName=middle&lastName=last&email=user@example.com](http://localhost.acikdemokrasi.org:8080/api/1/user/create?firstName=first&middleName=middle&lastName=last&email=user@example.com)

```
{
  "status":"Error",
  "message":"You are not logged in"
  "data": [ ]
}
```
```
{
  "status":"Error",
  "message":"Missing email address"
  "data": [ ]
}
```
```
{
  "status":"Error",
  "message":"E-mail address exists"
  "data": [ ]
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