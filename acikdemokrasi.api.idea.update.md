# Açıkdemokrasi API Doc - idea.update

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be the creator or an administrator
- Text should be minimum 5, maximum 500 long
- Hashtags in the text should be between '#' and ' '

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/idea/1/update?text=updatedText](http://localhost.acikdemokrasi.org:8080/api/1/idea/1/update?text=updatedText)

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
    "text":"updatedText",
    "tags":["tag1","tag2"],
    "upVotes":0,
    "downVotes":0,
    "voteScore":0,
    "created":"2013-07-11T00:24:54Z",
    "updated":"2013-07-11T00:24:54Z"
  }
}
```