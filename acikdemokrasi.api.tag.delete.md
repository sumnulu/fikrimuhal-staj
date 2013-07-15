# Açıkdemokrasi API Doc - tag.delete

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/tag/1/delete](http://localhost.acikdemokrasi.org:8080/api/1/tag/1/delete)

```
{
  "status":"Error",
  "message":"You are not logged in",
  "data": [ ]
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
  "status":"Error",
  "message":"Object not found",
  "data": [ ]
}
```
```
{
  "status":"OK,
  "data": [ ]
}
```