# Summary

---
# Notes

## Hashing Passwords
Add as `implementation` to `build.gradle`:
```java
org.springframework.security:spring-security-crypto
```

### BCryptPasswordEncoder
- Creates and verifies hashes
- Create variable and update constructor to compare:
```java
private static final BCryptPasswordEncoder encoder = new BCryptPasswordEncoder();

public User(String username, String password) {
   this.username = username;
   this.pwHash = encoder.encode(password);
}
```


---
# Related

---
# Reference

---

