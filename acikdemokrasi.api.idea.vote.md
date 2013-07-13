# Açıkdemokrasi API Doc - idea.vote

[Back to API docs home](Home)

### Requirements
- User should be logged in
- For yes vote, vote.value is 1, for no it is -1, to reset vote, it is 0

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/idea/1/vote/1](http://localhost.acikdemokrasi.org:8080/api/1/idea/1/vote/1)

```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"Error",
  "message":"Object not found"
}
```
```
{
  "status":"Error",
  "message":"User voted before"
}
```
```
{
  "status":"Error",
  "message":"Invalid vote value"
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