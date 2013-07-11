# Açıkdemokrasi API Doc - idea.delete

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator

### Example usage
```
http://localhost.acikdemokrasi.org:8080/ideaApi/delete?id=1
```
```
{
  "status":"Error",
  "message":"You are not logged in"
}
```
```
{
  "status":"Error",
  "message":"You do not have permission for this operation"
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
  "status":"OK
}
```