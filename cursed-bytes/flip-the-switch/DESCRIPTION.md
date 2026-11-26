Deep inside your device, all there is is a bunch of tiny switches called transistors. A switch has only 2 states. It can either be on or off.

```
        ON (1)                      OFF (0)

   o━━━━━━━━━━━━━━o            o━━━━━━━━╱     o

     high voltage                low voltage
```

The switch is considered on if it has a high voltage and off if it has a low voltage. We can represent something by a pattern of these on and off switches. For example, ON OFF OFF ON represents the digit 9 we know. Instead of saying ON and OFF every time, we just say 0 for off and 1 for on to save time. So we represent 9 by 1001, because all we've got at the end of the day is 1s and 0s.

Just 4 zeroes and ones can only make so many patterns. If you calculate, you can see there are only 16 possible patterns using 4 ones and zeroes, so we use 8 digits, which gives us 256 possible patterns (2⁸), so we can represent more things. This is the default thing we use for representing something generally. So, for example, 01001000 represents the letter H and 01101001 represents i.

Each of these 1s and 0s is called a bit, and we call this group of 8 bits a byte. A byte being 8 bits is a convention; early computers used other sizes.

Fun fact: if we wanted to say Hi using computers, we could say 01001000 01101001, which would mean Hi.

In computers, a byte is the smallest addressable unit for many reasons. One reason is that every slot in memory that stores something has an address (we will learn more about this later), and on 64-bit machines, every address is itself 8 bytes long. So if we could address one bit instead of one byte, we would need 8 times as many addresses for the same amount of memory.

This is just one of the many reasons we address only one byte at a time. Though, you can still change and perform operations on just a bit or a bunch of bits.

Now, one way to read these zeroes and ones, also known as binary, is to read them as numbers, just like our normal number system, except that there, each place is worth 10 times the place to its right, and here, it's worth just double.

**123 in decimal**

| Place value | 100 | 10 | 1 |
|---|---|---|---|
| Digit | 1 | 2 | 3 |
| Worth | 100 | 20 | 3 |

100 + 20 + 3 = **123**

**123 in binary (1111011)**

| Place value | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|
| Digit | 1 | 1 | 1 | 1 | 0 | 1 | 1 |
| Worth | 64 | 32 | 16 | 8 | 0 | 2 | 1 |

64 + 32 + 16 + 8 + 0 + 2 + 1 = **123**

Reading the digits is very easy: you just add all the place values where there is a 1.

**01001000**

| Place value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
|---|---|---|---|---|---|---|---|---|
| Digit | 0 | 1 | 0 | 0 | 1 | 0 | 0 | 0 |
| Worth | 0 | 64 | 0 | 0 | 8 | 0 | 0 | 0 |

64 + 8 = **72**

**Now the challenge:** read 3 4-bit numbers and 3 8-bit numbers. Run `/challenge/run` to start.
