# Açıkdemokrasi API Doc - tag.create

[Back to API docs home](Home)

### Requirements
- User should be logged in
- Text should be minimum 1, maximum 25 long

### Example usage

GET
>    http://localhost.acikdemokrasi.org:8080/api/1/tag/1

```
{
  "status":"Error",
  "message":"You are not logged in"
  "data": [ ]
}
```
```
{
  "status":"OK",
  "data": {
    "id":15,
    "name":"exampleTag",
    "style":null,
    "created":"2013-07-11T00:24:54Z",
    "updated":"2013-07-11T00:24:54Z"
  }
}
```