# Açıkdemokrasi API Doc - user.verifyEmail

[Back to API docs home](Home)

### Requirements
- Email address must not be verified before
- Email verification token should be valid

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/verifyEmail
- Content-Type: application/json
- Raw-body (data-binary): {"token":"e742da93-0fee-4d06-9561-0e03f3bec47b"}

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