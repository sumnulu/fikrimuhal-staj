# Açıkdemokrasi API Doc - idea.delete

[Back to API docs home](Home)

### Requirements
- User should be logged in
- User should be an administrator

### Example usage

- Request: DELETE
- Url: http://localhost.acikdemokrasi.org:8080/api/1/idea/1

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