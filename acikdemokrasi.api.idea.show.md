# Açıkdemokrasi API Doc - idea.show

[Back to API docs home](Home)

### Example usage
```
http://localhost.acikdemokrasi.org:8080/ideaApi/show?id=1
```
```
{
  "status":"Error",
  "message":"Object not found"
}
```
```
{
  "status":"OK",
  "data": {
    "author": {
      "id":1
    },
    "id":1,
    "text":"exampleidea",
    "tags":["tag1","tag2"],
    "upVotes":0,
    "downVotes":0,
    "voteScore":0,
    "created":"2013-07-11T00:24:54Z",
    "updated":"2013-07-11T00:24:54Z"
  }
}
```