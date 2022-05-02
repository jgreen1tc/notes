# <% tp.date.now("YYYY-MM-DD") %>
---

## Tasks ✅

### URGENT + IMPORTANT
*Do it now*


### URGENT, NOT IMPORTANT
*Delegate or do it after tasks above*


### IMPORTANT, NOT URGENT
*Decide when to do it*


### NOT URGENT, NOT IMPORTANT
*Do it later / Dump it*

--- 

### Overdue
```tasks
not done
due before <% tp.date.now("YYYY-MM-DD") %> 
```

### Due today
```tasks
not done
due on <% tp.date.now("YYYY-MM-DD") %> 
```
### Due tomorrow
```tasks
not done
due on <% tp.date.tomorrow("YYYY-MM-DD") %>
```
### Due next week
```tasks
not done
due after <% tp.date.tomorrow("YYYY-MM-DD") %>
due before <% tp.date.now("YYYY-MM-DD", +7) %>
```

### No due date
```tasks
not done
no due date
```


### Done today
```tasks
done on <% tp.date.now("YYYY-MM-DD") %> 
```
---


