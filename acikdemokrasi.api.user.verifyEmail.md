# Açıkdemokrasi API Doc - user.verifyEmail

[Back to API docs home](Home)

### Requirements
- Email address must not be verified before
- Email verification token should be valid

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/user/verifyEmail?token=9dbed920-1289-4426-972a-95149b1113be](http://localhost.acikdemokrasi.org:8080/api/1/user/verifyEmail?token=9dbed920-1289-4426-972a-95149b1113be)

```
{
  "status":"Error",
  "message":"Missing or wrong token",
  "code":999,
  "data": []
}
```
```
{
  "status":"Error",
  "message":"Email address already verified",
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