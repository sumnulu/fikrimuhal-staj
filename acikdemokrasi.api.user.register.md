# Açıkdemokrasi API Doc - user.register

[Back to API docs home](Home)

### Requirements
- Email and password fields should not be blank
- Email address should not be used before
- After the register, user will receive an email verification mail

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/register' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, */*' --data-binary '{"email":"test@example.com","password":"myPassword","firstName":"first","middleName":"middle","lastName":"last"}'

|

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
  message:"Email address exists",
  code: 651,
  data: []
}
```
```
{
  status:"Error",
  message:"Values are not valid",
  code: 633,
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