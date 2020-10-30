# 4 Stage = 4x Better

We are given the link:
```
https://chal.hackmac.xyz:30105
```
![1](1.jpg)

The title tells us we have 4 stages to get through.

**Stage 1:**

![2](2.jpg)

A caesar salad can only mean one thing - Caesar cipher. Running it through CyberChef (rotating through all the numbers until we reached a word) gives us:

`Germany`

![3](3.jpg)

**Stage 2:**

![4](4.jpg)

This definitely looks like morse code but running it through CyberChef gives us something that doesn't look right (confirmed by trying to submit it in the final flag).

![5](5.jpg)

Even trying to change the delimiter to a forward slash did not provide a result:

![6](6.jpg)

So, by manually checking each one against the morse code lookup table:

![7](7.jpg)

We got:

`Jamaica`

**Stage 3:**

![8](8.jpg)

This definitely looks like a substitution cipher, but it wasn't immediately clear that the 'hint' was actually a 'key'. After trying a couple of manual substitutions, we tried the Vigenere decode on it and it returned:

`Afghanistan`

![9](9.jpg)

**Stage 4:**

![10](10.jpg)

The weapon appears to be an MP5, and a hash brown likely means it relates to a hash. So by running the text we were given, on an MD5 hash decode lookup 
```
https://md5.gromweb.com/?md5=4647d00cf81f8fb0ab80f753320d0fc9
```

We get:

`Indonesia`

![11](11.jpg)


The next page shows us that the words we found are the flag:

![4](12.jpg)

```
hackmac{GermanyJamaicaAfghanistanIndonesia}
```