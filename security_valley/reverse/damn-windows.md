# Damn Windows

## Challenge

![](../images/damn-windows.png)

## Solution

The challenge gives us a PE32+ file `01.exe` and apparently it is "exotic" compilation. We open it with Ghidra and clearly see it's golang. <br>
We directly check main.main function:

![](../images/damn-windows2.png)

We understand that the function ask us for a password and read our input. <br>We see a function that seems to compare the password, thus we decide to inspect it to see if we can retrieve the string that is compared to our input:

![](../images/damn-windows3.png)

It's a bit messy we understand that it's doing comparison but cannot see the param which is compared to our input, we check the assembly code to check if we can see more informations:

![](../images/damn-windows4.png)

We clearly see that there is a string loaded in the stack, could it be the string we're looking for ? We check each DAT and the offset to recover the string:

![](../images/damn-windows5.png)

![](../images/damn-windows6.png)

![](../images/damn-windows7.png)

![](../images/damn-windows8.png)

That gives us:

`SecVal{this_1S_n1ce}`

Flagged !
