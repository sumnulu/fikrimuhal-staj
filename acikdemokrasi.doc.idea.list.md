# Açıkdemokrasi API DOC - 

[Back to API docs home](Home)

### Example usage
```
http://localhost.acikdemokrasi.org:8080/ideaApi/list
http://localhost.acikdemokrasi.org:8080/ideaApi/list?since=2013-06-06
http://localhost.acikdemokrasi.org:8080/ideaApi/list?author=2
http://localhost.acikdemokrasi.org:8080/ideaApi/list?voted
http://localhost.acikdemokrasi.org:8080/ideaApi/list??tags=tag1,tag2
```
```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"OK",
  "data": [
    {
      "author":{
        "id":1
      },
      "id":1,
      "text":"Idea1",
      "tags":["tag1","tag2"],
      "upVotes":0,
      "downVotes":0,
      "voteScore":0,
      "created":"2013-07-10T18:10:46Z",
      "updated":"2013-07-10T18:10:46Z"
    }
    ..
  ]
}
```