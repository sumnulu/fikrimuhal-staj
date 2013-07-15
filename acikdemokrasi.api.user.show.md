# Açıkdemokrasi API Doc - idea.show

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not admin only current user's info returns, otherwise user info returns

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/idea/1/show](http://localhost.acikdemokrasi.org:8080/api/1/idea/1/show)

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
    "totalTopics":4
  }
}
```