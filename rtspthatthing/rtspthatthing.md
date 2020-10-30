# RTSP That Thing

From the challenge description, we can find some useful pieces of information:
 - We're looking for an RTSP stream
 - The stream is unencrypted
 - The brand of camera is Zmodo

Let's first have a look at what ports we should be scanning. A quick google search for `Zmodo RTSP` shows some common URLs used by Zmodo cameras to display their RTSP feeds. They appear to use the port 10554.

We can do an nmap scan of the network to find hosts with this port open.

Now that we have the host address, we can try some of the common URLs in VLC to get the RTSP stream.

```
rtsp://192.168.100.210:10554/udp/av0_0
```
This gives us a video stream, and the flag is written on a piece of paper.