# Intelli-telnet

This challenge is relatively simple. The description gives us a great deal of information:

 - The telnet password is the device's default
 - The device is a Zmodo camera
 - The flag is the password (in the flag format)

A quick google search shows reports of a telnet password for this device being

```
zmodo19820816
```

Attempting to connect to the host with this password shows that this is the correct password, so the flag is `hackmac{zmodo19820816}`.