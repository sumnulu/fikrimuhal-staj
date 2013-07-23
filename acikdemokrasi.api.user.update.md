# Açıkdemokrasi API Doc - idea.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not administrator, user can only edit his own records

### Example usage

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/user/977/update' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, */*' --data-binary '{"firstName":"newFirst","middleName":"newMiddle","lastName":"newLast"}'

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