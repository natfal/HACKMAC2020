# Smart Camera Secret File

This challenge is a continuation of [Intelli-telnet](../intellitelnet/intellitelnet.md). Firstly, we need to connect to the camera with Telnet using the password from the previous challenge.

Once we are in, we can start looking for the hidden file mentioned in the challenge description.

```
$ ls -a
```

Nothing of note is found in this directory, so we can navigate up a directory and list the files

```
$ cd ..
$ ls -a
```

Here, we can see a file of note. We can access the contents of the file:

```
$ cat flag.txt
```

And the flag is printed to the terminal!