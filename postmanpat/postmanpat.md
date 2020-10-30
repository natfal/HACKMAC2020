# Postman Pat knows everything about 13 Rotten Apples

On Jeffery's Twitter we can see he has a follower called "Aaron Boolon" who is also a fake account created for Hackmac:

![1](1.jpg)

We could see his first post referred to `"13 ROTten Apples"`, so we knew it was likely to be related to this challenge.

![2](2.jpg)

We could see an encrypted message in the form of a hyperlink (due to the `://`)

Using Cyberchef, and decoding ROT13:

![3](3.jpg)

We get a new hackmac website:

```
http://badboys.hackmac.xyz
```
On the website, we see an option that says `flag`:

![4](4.jpg)

Of course, we click on this and we get something in the hackmac flag format:

![5](5.jpg)

```
hackmac{hello_mr_postman}
```