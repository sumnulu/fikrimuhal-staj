# Açıkdemokrasi API Doc - user.showProfile

[Back to API docs home](Home)

### Example usage

- Request: GET
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/profile?ids=1,2

```
{
  "status":"OK",
  "data": [
    {
      "facebook": [
        "id":1
      ]
      "id":1,
      "fullName":"first middle last",
      "pictureUrl":"",
      "type":"Vatandaş",
    }
    ..
  ]
}
```