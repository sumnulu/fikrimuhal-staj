# Açıkdemokrasi API Doc - tag.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator
- Text should be minimum 1, maximum 500 long

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/tag/1/update?text=updatedName](http://localhost.acikdemokrasi.org:8080/api/1/tag/1/update?text=updatedName)

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
    "id":15,
    "name":"updatedName",
    "style":null
  }
}
```