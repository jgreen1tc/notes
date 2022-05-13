# Summary

---
# Notes

## Creating the UserRepository
- Needed in order to access User objects stored in the database
```java
public interface UserRepository extends CrudRepository<User, Integer> {

   User findByUsername(String username);

}
```


---
# Related
[[User Model]]

---
# Reference

---

