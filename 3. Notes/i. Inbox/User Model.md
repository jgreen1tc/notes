# Summary

---
# Notes
## Sample User Model
```java
@Entity
public class User extends AbstractEntity {

   @NotNull
   private String username;

   @NotNull
   private String pwHash;

   public User() {}

   public User(String username, String password) {
	   this.username = username;
	   this.pwHash = password;
   }

   public String getUsername() {
	   return username;
   }
   
// Salting carried out by encoder.matches() before comparison
   public boolean isMatchingPassword(String password) {
	   return encoder.matches(password, pwHash);
   }




}
```

Notice that the constructor takes a parameter named password and uses it to set the value of pwHash. We mentioned previously that we should never store passwords, so in a moment, we will update line 26 by creating a hash from the given password to store.


---
# Related
[[User Authentication]]
[[Hashing Passwords]]
[[User Repository]]


---
# Reference
[Creating a User Model](https://education.launchcode.org/java-web-development/chapters/auth/user-model.html#:~:text=A%20model%20class%20representing%20users,string%20fields%2C%20username%20and%20pwHash%20.)

---

