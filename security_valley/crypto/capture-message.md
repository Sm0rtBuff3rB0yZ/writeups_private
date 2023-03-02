# Capture message

## Challenge

![](../images/capture-message1.png)

# Solution

The challenge provides us with a text file containing a message that appears to be ciphered with `Cesar code`

![](../images/capture-message2.png)

We then write a brute-force in `bash` to test the 26 possibilities:

![](../images/capture-message3.png)

We filter the output with a `grep` to try to get a flag:

![](../images/capture-message4.png)

Bingo!
