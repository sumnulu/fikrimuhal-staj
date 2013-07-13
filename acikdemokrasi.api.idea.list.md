# Açıkdemokrasi API Doc - idea.list

[Back to API docs home](Home)

### Requirements
- If author filter used, user should be logged in
- If author filter used and user is not admin, only logged in user's records will show up. Otherwise, all records will show up.

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/idea/list](http://localhost.acikdemokrasi.org:8080/api/1/idea/list)
[http://localhost.acikdemokrasi.org:8080/api/1/idea/list?since=2013-06-06](http://localhost.acikdemokrasi.org:8080/api/1/idea/list?since=2013-06-06)
[http://localhost.acikdemokrasi.org:8080/api/1/idea/list?author=1](http://localhost.acikdemokrasi.org:8080/api/1/idea/list?author=1)
[http://localhost.acikdemokrasi.org:8080/api/1/idea/list?voted](http://localhost.acikdemokrasi.org:8080/api/1/idea/list?voted)
[http://localhost.acikdemokrasi.org:8080/api/1/idea/list?tags=tag1,tag2](http://localhost.acikdemokrasi.org:8080/api/1/idea/list?tags=tag1,tag2)

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