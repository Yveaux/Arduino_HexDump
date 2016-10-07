# Arduino_HexDump
An Arduino library for hexadecimal/ASCII dumping of data

A typical example to dump a block of data to the serial console:

```
uint8_t data[100];

HexDump(Serial, data, sizeof(data));
```
