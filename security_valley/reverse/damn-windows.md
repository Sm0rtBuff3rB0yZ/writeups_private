# Damn Windows

## Challenge

![](../images/damn-windows.png)

## Solution

The challenge gives us a PE32+ file `01.exe` and apparently it is "exotic" compilation. We open it with Ghidra and directly check main.main function:

![](../images/the-loader2.png)

