# Damn Windows

## Challenge

![](../images/damn-windows.png)

## Solution

The challenge gives us a PE32+ file `01.exe` and apparently it is "exotic" compilation. We open it with Ghidra and directly check main.main function:

![](../images/damn-windows2.png)

![](../images/damn-windows3.png)

![](../images/damn-windows4.png)

