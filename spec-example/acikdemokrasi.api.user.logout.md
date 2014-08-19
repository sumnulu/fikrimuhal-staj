# Açıkdemokrasi API Doc - user.logout

[Back to API docs home](Home)

### Requirements
- User should be logged in

### Example usage

[http://localhost.acikdemokrasi.org:8080/api/1/user/logout](http://localhost.acikdemokrasi.org:8080/api/1/user/logout)

```
{
  status:"Error",
  message:"You are not logged in",
  code: 610,
  data: []
}
```
```
{
  status:"OK",
  message: "User logged out successfuly"
}
```