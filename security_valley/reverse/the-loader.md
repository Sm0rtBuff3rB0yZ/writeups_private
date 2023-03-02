# The Loader

## Challenge

![](../images/the-loader1.png)

## Solution

We open the given ELF binary (crackme-03) inside Ghidra and directly open main function:

![](../images/the-loader2.png)

We see a weird parameter `local_18` used in the very sus function `huuu(local_18)` so we decide to dig a bit: 

![](../images/the-loader3.png)

![](../images/the-loader4.png)

