# Açıkdemokrasi API Doc - tag.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator
- Text should be minimum 1, maximum 25 long

### Example usage

- Request: POST
- Url: http://localhost.acikdemokrasi.org:8080/api/1/tag/1
- Content-Type: application/json
- Raw-body (data-binary): {"name":"updatedName"}

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
    "id":1,
    "name":"updatedName",
    "style":null,
    "created":"2013-07-11T00:24:54Z",
    "updated":"2013-07-11T00:24:54Z"
  }
}
```