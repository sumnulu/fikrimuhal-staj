# Açıkdemokrasi API Doc - user.list

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator
- Max 25 records are shown
- If page parameter is not set shows first page

### Example usage

- [http://localhost.acikdemokrasi.org:8080/api/1/user/list](http://localhost.acikdemokrasi.org:8080/api/1/user/list)
- [http://localhost.acikdemokrasi.org:8080/api/1/user/list?page=2](http://localhost.acikdemokrasi.org:8080/api/1/user/list?page=2)

```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"Error",
  "message":"You do not have permission for this operation",
  "data": [ ]
}
```
```
{
  "status":"OK",
  "data": [
    {
      "facebook": [
        "id":1
      ]
      "id":1,
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
    ..
  ]
}
```