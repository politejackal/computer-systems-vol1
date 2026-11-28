Alright, now recall I said we represent different stuff by a pattern of on or off switches. Well, here we are gonna do exactly that!

Characters are represented with a pattern of these zeroes and ones. For example, 01000001 represents A. But 01000001 also means 0x41 in hex, and 65 in decimal! And if you read those same digits as a decimal number, it would just be one million and one! Well, you see, it's only a matter of how we see these zeroes and ones that decides what they mean. So another way to see these zeroes and ones is ASCII (American Standard Code for Information Interchange), which is an agreed-upon convention that such and such zeroes and ones represent such and such characters.

ASCII uses only 7 bits, so it has 128 characters, from 0x00 to 0x7f. Each character is stored in one byte.

Here is the table:

| Binary | Decimal | Hex | Character |
|---|---|---|---|
| 00000000 | 0 | 0x00 | NUL (`\0`) |
| 00000001 | 1 | 0x01 | SOH |
| 00000010 | 2 | 0x02 | STX |
| 00000011 | 3 | 0x03 | ETX |
| 00000100 | 4 | 0x04 | EOT |
| 00000101 | 5 | 0x05 | ENQ |
| 00000110 | 6 | 0x06 | ACK |
| 00000111 | 7 | 0x07 | BEL |
| 00001000 | 8 | 0x08 | BS |
| 00001001 | 9 | 0x09 | HT (`\t`) |
| 00001010 | 10 | 0x0a | LF (`\n`) |
| 00001011 | 11 | 0x0b | VT |
| 00001100 | 12 | 0x0c | FF |
| 00001101 | 13 | 0x0d | CR (`\r`) |
| 00001110 | 14 | 0x0e | SO |
| 00001111 | 15 | 0x0f | SI |
| 00010000 | 16 | 0x10 | DLE |
| 00010001 | 17 | 0x11 | DC1 |
| 00010010 | 18 | 0x12 | DC2 |
| 00010011 | 19 | 0x13 | DC3 |
| 00010100 | 20 | 0x14 | DC4 |
| 00010101 | 21 | 0x15 | NAK |
| 00010110 | 22 | 0x16 | SYN |
| 00010111 | 23 | 0x17 | ETB |
| 00011000 | 24 | 0x18 | CAN |
| 00011001 | 25 | 0x19 | EM |
| 00011010 | 26 | 0x1a | SUB |
| 00011011 | 27 | 0x1b | ESC |
| 00011100 | 28 | 0x1c | FS |
| 00011101 | 29 | 0x1d | GS |
| 00011110 | 30 | 0x1e | RS |
| 00011111 | 31 | 0x1f | US |
| 00100000 | 32 | 0x20 | (space) |
| 00100001 | 33 | 0x21 | ! |
| 00100010 | 34 | 0x22 | " |
| 00100011 | 35 | 0x23 | `#` |
| 00100100 | 36 | 0x24 | $ |
| 00100101 | 37 | 0x25 | % |
| 00100110 | 38 | 0x26 | & |
| 00100111 | 39 | 0x27 | ' |
| 00101000 | 40 | 0x28 | ( |
| 00101001 | 41 | 0x29 | ) |
| 00101010 | 42 | 0x2a | `*` |
| 00101011 | 43 | 0x2b | + |
| 00101100 | 44 | 0x2c | , |
| 00101101 | 45 | 0x2d | - |
| 00101110 | 46 | 0x2e | . |
| 00101111 | 47 | 0x2f | / |
| 00110000 | 48 | 0x30 | 0 |
| 00110001 | 49 | 0x31 | 1 |
| 00110010 | 50 | 0x32 | 2 |
| 00110011 | 51 | 0x33 | 3 |
| 00110100 | 52 | 0x34 | 4 |
| 00110101 | 53 | 0x35 | 5 |
| 00110110 | 54 | 0x36 | 6 |
| 00110111 | 55 | 0x37 | 7 |
| 00111000 | 56 | 0x38 | 8 |
| 00111001 | 57 | 0x39 | 9 |
| 00111010 | 58 | 0x3a | : |
| 00111011 | 59 | 0x3b | ; |
| 00111100 | 60 | 0x3c | `<` |
| 00111101 | 61 | 0x3d | = |
| 00111110 | 62 | 0x3e | `>` |
| 00111111 | 63 | 0x3f | ? |
| 01000000 | 64 | 0x40 | @ |
| 01000001 | 65 | 0x41 | A |
| 01000010 | 66 | 0x42 | B |
| 01000011 | 67 | 0x43 | C |
| 01000100 | 68 | 0x44 | D |
| 01000101 | 69 | 0x45 | E |
| 01000110 | 70 | 0x46 | F |
| 01000111 | 71 | 0x47 | G |
| 01001000 | 72 | 0x48 | H |
| 01001001 | 73 | 0x49 | I |
| 01001010 | 74 | 0x4a | J |
| 01001011 | 75 | 0x4b | K |
| 01001100 | 76 | 0x4c | L |
| 01001101 | 77 | 0x4d | M |
| 01001110 | 78 | 0x4e | N |
| 01001111 | 79 | 0x4f | O |
| 01010000 | 80 | 0x50 | P |
| 01010001 | 81 | 0x51 | Q |
| 01010010 | 82 | 0x52 | R |
| 01010011 | 83 | 0x53 | S |
| 01010100 | 84 | 0x54 | T |
| 01010101 | 85 | 0x55 | U |
| 01010110 | 86 | 0x56 | V |
| 01010111 | 87 | 0x57 | W |
| 01011000 | 88 | 0x58 | X |
| 01011001 | 89 | 0x59 | Y |
| 01011010 | 90 | 0x5a | Z |
| 01011011 | 91 | 0x5b | `[` |
| 01011100 | 92 | 0x5c | `\` |
| 01011101 | 93 | 0x5d | `]` |
| 01011110 | 94 | 0x5e | ^ |
| 01011111 | 95 | 0x5f | `_` |
| 01100000 | 96 | 0x60 | `` ` `` |
| 01100001 | 97 | 0x61 | a |
| 01100010 | 98 | 0x62 | b |
| 01100011 | 99 | 0x63 | c |
| 01100100 | 100 | 0x64 | d |
| 01100101 | 101 | 0x65 | e |
| 01100110 | 102 | 0x66 | f |
| 01100111 | 103 | 0x67 | g |
| 01101000 | 104 | 0x68 | h |
| 01101001 | 105 | 0x69 | i |
| 01101010 | 106 | 0x6a | j |
| 01101011 | 107 | 0x6b | k |
| 01101100 | 108 | 0x6c | l |
| 01101101 | 109 | 0x6d | m |
| 01101110 | 110 | 0x6e | n |
| 01101111 | 111 | 0x6f | o |
| 01110000 | 112 | 0x70 | p |
| 01110001 | 113 | 0x71 | q |
| 01110010 | 114 | 0x72 | r |
| 01110011 | 115 | 0x73 | s |
| 01110100 | 116 | 0x74 | t |
| 01110101 | 117 | 0x75 | u |
| 01110110 | 118 | 0x76 | v |
| 01110111 | 119 | 0x77 | w |
| 01111000 | 120 | 0x78 | x |
| 01111001 | 121 | 0x79 | y |
| 01111010 | 122 | 0x7a | z |
| 01111011 | 123 | 0x7b | { |
| 01111100 | 124 | 0x7c | \| |
| 01111101 | 125 | 0x7d | } |
| 01111110 | 126 | 0x7e | ~ |
| 01111111 | 127 | 0x7f | DEL |

The table starts with some non-printable characters, from 0x00 to 0x1f, and 0x7f at the very end. These are not meant to be shown on the screen. Instead, they control things, like 0x0a (`\n`), which starts a new line.

But notice that the uppercase letters start from 0x41 in hex, and the lowercase letters start from 0x61. I am saying hex because hex is king, and everybody uses hex, and you will use it too in the near future!

Some patterns worth noticing:

- Uppercase and lowercase letters are exactly 0x20 apart: A is 0x41 and a is 0x61. Only one bit is different!
- The character '0' is 0x30, not 0x00. The character '0' and the number 0 are not the same thing.
- 0x00 (`\0`), 0x0a (`\n`) and 0x20 (space) are special bytes you will meet again and again when sending input to programs.
- If you ever see 0x41414141 somewhere, that is just AAAA. Hackers love sending lots of A's so they can spot their own input in memory. Anyway don't worry about this memory and all for now!

You can always see this table on Linux by running `man ascii`.
