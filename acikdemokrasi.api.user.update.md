# Açıkdemokrasi API Doc - idea.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not administrator, user can only edit his own records

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/1/update 
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/update (current user)

- Content-Type: application/json
- Raw-body (data-binary): {"firstName":"newFirst","middleName":"newMiddle","lastName":"newLast"}

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
    "totalTopics":4,
    "isAdmin":1
  }
}
```