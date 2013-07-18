# Açıkdemokrasi API Doc - user.list

[Back to API docs home](Home)

### Requirements
- User should be logged in
- If not administrator, user can only edit his own records

### Example usage

- [http://localhost.acikdemokrasi.org:8080/api/1/idea/1/vote/1](http://localhost.acikdemokrasi.org:8080/api/1/idea/1/vote/1)

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
    {
      "idea":{
        "id":1,
        "text":"Ergenekon ve balyoz davaları"
      },
      "value":1
    }
    ..
  ]
}
```