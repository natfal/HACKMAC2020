# Time for a Little Magic Trick

Trying to open Joker.db in database software reveals it's not actually a database. To see what is actually in the `.db` file 

```bash
$ binwalk Joker.db
```  
will reveal jpg data in database file.  
```
$   binwalk -D='.*' Joker.db
```

extracts jpg image of a joker card with flag written at the top.
