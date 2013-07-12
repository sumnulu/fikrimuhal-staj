# Açıkdemokrasi API Doc - idea.create

[Back to API docs home](Home)

### Requirements
- User should be logged in
- Text should be minimum 5, maximum 500 long
- Hashtags in the text should be between '#' and ' '

### Example usage
```
[xxx](http://localhost.acikdemokrasi.org:8080/ideaApi/create?text=exampleidea)
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