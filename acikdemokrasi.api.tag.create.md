# Açıkdemokrasi API Doc - tag.create

[Back to API docs home](Home)

### Requirements
- User should be logged in
- Text should be minimum 1, maximum 25 long

### Example usage

- Request: PUT
- Url: http://localhost.acikdemokrasi.org:8080/api/1/tag
- Content-Type: application/json
- Raw-body (data-binary): {"name":"updatedName"}

>    curl 'http://localhost.acikdemokrasi.org:8080/api/1/tag/create' -H 'Content-Type: application/json;charset=UTF-8' -H 'Accept: application/json, text/plain, /' --data-binary '{"name":"testTag"}'

|
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