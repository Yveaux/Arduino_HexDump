# Arduino_HexDump
An Arduino library for hexadecimal/ASCII dumping of data

A typical example to dump a block of data to the serial console:

```
uint8_t data[100];

HexDump(Serial, data, sizeof(data));
```

The generated hexadecimal dump will be something like (data is wav file header on ESP8266):

```
00000000: 52 49 46 46 00 00 00 00 57 41 56 45 66 6D 74 20  RIFF....WAVEfmt 
00000010: 12 00 00 00 01 00 01 00 44 AC 00 00 88 58 01 00  ........D¬..ˆX..
00000020: 02 00 10 00 00 00 4C 49 53 54 1A 00 00 00 49 4E  ......LIST....IN
00000030: 46 4F 49 53 46 54 0E 00 00 00 4C 61 76 66 35 35  FOISFT....Lavf55
00000040: 2E 31 38 2E 31 30 32 00 64 61 74 61 00 00 00 00  .18.102.data....
00000050: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00  ................
00000060: 00 00 00 00                                      ....
```
