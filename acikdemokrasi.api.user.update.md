# Açıkdemokrasi API Doc - idea.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not administrator, user can only edit his own records

### Example usage


[http://localhost.acikdemokrasi.org:8080/api/1/user/1/update?firstName=first&middleName=middle&lastName=last](http://localhost.acikdemokrasi.org:8080/api/1/user/1/update?firstName=first&middleName=middle&lastName=last)

```
{
  "status":"Error",
  "message":"Object not found",
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
    "totalTopics":4
  }
}
```