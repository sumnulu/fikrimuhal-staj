# Açıkdemokrasi API Doc - tag.list

[Back to API docs home](Home)

### Example usage

- Request: GET
- Url: http://localhost.acikdemokrasi.org:8080/api/1/tag

```
{
  "status":"Error",
  "message":"You are not logged in",
  "data": [ ]
}
```
```
{
  "status":"OK",
  "data": [
    {
      "id":1,
      "name":"exampleTag",
      "style":null,
      "created":"2013-07-11T00:24:54Z",
      "updated":"2013-07-11T00:24:54Z"
    }
    ..
  ]
}
```