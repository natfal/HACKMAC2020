# Time for a Little Magic Trick

Trying to open Joker.db in database software reveals it's not actually a database. 

![opening in database software](1.png)

To see what is actually in the `.db` file, we can run

```bash
$ binwalk Joker.db
```  
This will reveal the true contents of the file

![binwalk](2.png)

As we can see, the file has a JPEG image hidden within. To see the actual image, we need to extract it from the carrier file 

```bash
$   binwalk -D='.*' Joker.db
```

This will put the contents of the file in a new folder

![extracted files](3.png)

From here, we can simply open the file with an image viewer of choice

![flag](4.png)

And we have our flag!