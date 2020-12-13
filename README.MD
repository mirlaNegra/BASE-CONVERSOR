# BASE-CONVERSOR
This vbs script converts the base of a number between the hexadecimal, octal, decimal, and binary base.

## Logic of the Vbs Script BASE-CONVERSOR
*Every dec-bin result on 3, 4, 7 and 8 must be four digit wide on hex and three digit wide on oct
*

1. dec > hex or oct or bin
Example: 
1.(D/16)
2.((D/16))/16
3.((D/16)/16)/16
4.(((D/16)/16)/16)/16
5.((((D/16)/16)/16)/16)/16
...
n.1/16 = 1

HEX= ResidueN Residue5 Residue4 Residue3 Residue2 Residue1

2. bin-dec
DEC= binn * 2n-1 