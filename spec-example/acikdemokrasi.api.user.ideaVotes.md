# Açıkdemokrasi API Doc - user.ideaVotes

[Back to API docs home](Home)

### Requirements
- User should be logged in

### Example usage

- Request: GET
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/1/ideaVotes
- Url: http://localhost.acikdemokrasi.org:8080/api/1/user/ideaVotes  (current user)

```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"Error",
  "message":"You do not have permission for this operation",
  "data": [ ]
}
```
```
{
  "status":"OK",
  "data":[
         {idea:{id:4}, value:1}, {idea:{id:5}, value:1}, {idea:{id:26}, value:1}, {idea:{id:23}, value:1},
          …]
}
```