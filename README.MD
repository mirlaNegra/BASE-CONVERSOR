# BASE-CONVERSOR
This powershell script converts the base of a number between the hexadecimal, octal, decimal, and binary base.

## Logic of the Vbs Script BASE-CONVERSOR
*Every dec-bin result on 3, 4, 7 and 8 must be four digit wide on hex and three digit wide on oct
*Potentiation(x^n) - Multiplication(x * n) - Division(x / n) - Index(x(n))

1. dec-hex or oct or bin (Esencial)
Example: 
1.(D/16)
2.((D/16))/16
3.((D/16)/16)/16
4.(((D/16)/16)/16)/16
5.((((D/16)/16)/16)/16)/16
...
n.n/16 = 1

hex = ResidueN Residue5 Residue4 Residue3 Residue2 Residue1

2. bin-dec (Esencial)
*n = Binary number length
dec= bin(1) * 2^1-1 + bin(2) * 2^2-1 + bin(3) * 2^3-1 + bin(4) * 2^4-1 + bin(5) * 2^5-1 + ... + bin(n) * 2^n-1

3. hex-dec
dec = bin-dec(dec-bin(hex1) & dec-bin(hex2) & dec-bin(hex3) & dec-bin(hex4) & dec-bin(hex5) & ... & dec-bin(hexn))

4. oct-dec
dec = bin-dec(dec-bin(oct1) & dec-bin(oct2) & dec-bin(oct3) & dec-bin(oct4) & dec-bin(oct5) & ... & dec-bin(octn))

5. oct-hex
hex = dec-hex(oct-dec(oct))

6. hex-oct 
oct = dec-oct(hex-dec(hex))

7. hex-bin
bin = dec-bin(hex1) & dec-bin(hex2) & dec-bin(hex3) & dec-bin(hex4) & dec-bin(hex5) & ... & dec-bin(hexn)

8. oct-bin
bin = dec-bin(oct1) & dec-bin(oct2) & dec-bin(oct3) & dec-bin(oct4) & dec-bin(oct5) & ... & dec-bin(octn)

9. bin-oct
oct = bin-dec(bin(1) & bin(2) & bin(3)) & dec-bin(bin(4) & bin(5) & bin(6)) & ... & dec-bin(bin(n-2) & bin(n-1) & bin(n))

10. bin-hex
hex = bin-dec(bin(1) & bin(2) & bin(3) & bin(4)) & bin-dec(bin(5) & bin(6) & bin(7) & bin(8)) & ... & dec-bin(bin(n-3) & bin(n-2) & bin(n-1) & bin(n))