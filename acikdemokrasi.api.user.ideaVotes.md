# Açıkdemokrasi API Doc - user.ideaVotes

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not administrator, user can only edit his own records

### Example usage

- [http://localhost.acikdemokrasi.org:8080/api/1/user/ideaVotes](http://localhost.acikdemokrasi.org:8080/api/1/user/ideaVotes)

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