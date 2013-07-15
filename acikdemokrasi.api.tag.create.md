# Açıkdemokrasi API Doc - tag.create

[Back to API docs home](Home)

### Requirements
- User should be logged in
- Text should be minimum 1, maximum 500 long

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/tag/create?name=exampleTag](http://localhost.acikdemokrasi.org:8080/api/1/tag/create?name=exampleTag)

```
{
  "status":"Error",
  "message":"You are not logged in"
  "data": []
}
```
```
{
  "status":"OK",
  "data": {
    "id":15,
    "name":"exampleTag",
    "style":null
  }
}
```