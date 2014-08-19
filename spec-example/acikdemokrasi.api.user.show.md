# Açıkdemokrasi API Doc - user.show

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not admin only current user's info returns, otherwise user info returns

### Example usage

- Request: GET
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/1
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user (current user)

```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"Error",
  "message":"Object not found",
  "data": []
}
```
```
{
  "status":"Error",
  "message":"You do not have permission for this operation",
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