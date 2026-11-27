Recall that decimal is the normal number system we use, with each place value 10 times bigger as we move from right to left. Also recall that binary is the place value system where each place value is double the one on its right.

Now recall how many patterns 4 bits can store. Sixteen! So we can represent a value from 0 to 15. Now, instead of using 4 characters, we made a shortcut: use just one character to represent something from 0 to 15. And mathematically, naturally, each digit place of this number system multiplies by 16. This number system is known as hexadecimal, or hex for short.

Now let's talk about the characters. For 0 to 9, we use the same characters, but for the remaining 6 characters, we extend and just use A to F.

So the characters go like:

| Hex | Decimal | Binary |
|---|---|---|
| 0 | 0 | 0000 |
| 1 | 1 | 0001 |
| 2 | 2 | 0010 |
| 3 | 3 | 0011 |
| 4 | 4 | 0100 |
| 5 | 5 | 0101 |
| 6 | 6 | 0110 |
| 7 | 7 | 0111 |
| 8 | 8 | 1000 |
| 9 | 9 | 1001 |
| A | 10 | 1010 |
| B | 11 | 1011 |
| C | 12 | 1100 |
| D | 13 | 1101 |
| E | 14 | 1110 |
| F | 15 | 1111 |

So one hex digit represents 4 bits. 8 bits make 1 byte, so 2 hex digits represent 1 byte. Remember it, it will come in handy: every byte you see in a memory dump, a debugger, or an exploit is written as exactly 2 hex digits, like `41` or `ff`.

To convert binary to hex, break the binary into 4-bit chunks, **starting from the right**. If the leftmost chunk has fewer than 4 bits, add zeroes to its left. Then just calculate each chunk in decimal, and whatever it is from 0 to 15, use the hex character for that value. Do that for each chunk, and you can convert any big number from binary to hex.

| Binary | 10 1101 |
|---|---|
| Chunks | 0010 1101 |
| Hex | 2 D |

So 0b101101 is **0x2D**.

Converting hex to decimal is similar to reading any place value number system. The first, or rightmost, digit is worth 16⁰ (1), the next digit to its left is worth 16¹ (16), then 16² (256), and so on. You multiply each digit by its place value and add them all up.

**0x1A3 to decimal**

| Place value | 256 (16²) | 16 (16¹) | 1 (16⁰) |
|---|---|---|---|
| Digit | 1 | A (10) | 3 |
| Worth | 256 | 160 | 3 |

256 + 160 + 3 = **419**

To convert hex to binary, just do the opposite of binary to hex: replace each hex digit with its 4 bits.

| Hex | 2 | D |
|---|---|---|
| Binary | 0010 | 1101 |

So 0x2D is **0b00101101**.

Now, just like the prefix 0b stands for binary, hex has the prefix 0x! Also, hex doesn't care about uppercase or lowercase: 0xFF and 0xff are the same. Most hacking tools print it in lowercase.

**Now the challenge:** convert 3 binary numbers to hex, then 3 hex numbers to binary. Run `/challenge/run_hexed` to start.
