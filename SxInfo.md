## About SnakeCrypt

SnakeCrypt encodes and decodes Sx64 (a custom codec made by me)

The number in each name (e.g. Sx<b>10</b>, Sx<b>16</b>)
identifies the [radix](https://en.wikipedia.org/wiki/Radix) used. Sx10 is considered the base one as all the formulas
extend from it

## Sx10 Formula

<code>x</code> is a placeholder for the current number

After each formula iteration <code>x</code> goes up by the next power of 2

Each formula iteration consists of the following:

```
000 => 00x => 0x0 => 0xx,
x00 => x0x => xx0 => xxx
```

## Sx16 Formula

The Sx16 formula is the same as the Sx10 formula however the final Sx10 values are converted from radix 10 to radix 16

## Sx10 Character Mappings

| Character | Sx10 Value   |
|-----------|--------------|
| 0         | 000          |
| 1         | 001          |
| 2         | 010          |
| 3         | 011          |
| 4         | 100          |
| 5         | 101          |
| 6         | 110          |
| 7         | 111          |
| 8         | 002          |
| 9         | 020          |
| A         | 022          |
| B         | 200          |
| C         | 202          |
| D         | 220          |
| E         | 222          |
| F         | 004          |
| G         | 040          |
| H         | 044          |
| I         | 400          |
| J         | 404          |
| K         | 440          |
| L         | 444          |
| N         | 008          |
| O         | 080          |
| P         | 088          |
| Q         | 800          |
| R         | 808          |
| S         | 880          |
| T         | 888          |
| U         | 0016         |
| V         | 0160         |
| W         | 01616        |
| X         | 1600         |
| Y         | 16016        |
| Z         | 16160        |
| a         | 161616       |
| b         | 0032         |
| c         | 0320         |
| d         | 03232        |
| e         | 3200         |
| f         | 32032        |
| g         | 32320        |
| h         | 323232       |
| i         | 0064         |
| j         | 0640         |
| k         | 06464        |
| l         | 6400         |
| m         | 64064        |
| n         | 64640        |
| o         | 646464       |
| p         | 00128        |
| q         | 01280        |
| r         | 0128128      |
| s         | 12800        |
| t         | 1280128      |
| u         | 1281280      |
| v         | 128128128    |
| w         | 00256        |
| x         | 02560        |
| y         | 0256256      |
| z         | 25600        |
| !         | 2560256      |
| "         | 2562560      |
| #         | 256256256    |
| $         | 00512        |
| %         | 05120        |
| &         | 0512512      |
| '         | 51200        |
| (         | 5120512      |
| )         | 5125120      |
| *         | 512512512    |
| +         | 001024       |
| ,         | 010240       |
| -         | 010241024    |
| .         | 102400       |
| /         | 102401024    |
| :         | 102410240    |
| ;         | 102410241024 |
| <         | 002048       |
| =         | 020480       |
| \>        | 020482048    |
| ?         | 204800       |
| @         | 204802048    |
| [         | 204820480    |
| \         | 204820482048 |
| ]         | 004096       |
| ^         | 040960       |
| _         | 040964096    |
| `         | 409600       |
| {         | 409604096    |
| \|        | 409640960    |
| }         | 409640964096 |
| ~         | 008192       |
|           | 081920       |

## Sx16 Character Mappings

| Character | Sx64 Value     |
|-----------|----------------|
| 0         | 0              |
| 1         | 1              |
| 2         | 16             |
| 3         | 17             |
| 4         | 256            |
| 5         | 257            |
| 6         | 272            |
| 7         | 273            |
| 8         | 2              |
| 9         | 32             |
| A         | 34             |
| B         | 512            |
| C         | 514            |
| D         | 544            |
| E         | 546            |
| F         | 4              |
| G         | 64             |
| H         | 68             |
| I         | 1024           |
| J         | 1028           |
| K         | 1088           |
| L         | 1092           |
| N         | 8              |
| O         | 128            |
| P         | 136            |
| Q         | 2048           |
| R         | 2056           |
| S         | 2176           |
| T         | 2184           |
| U         | 22             |
| V         | 352            |
| W         | 5654           |
| X         | 5632           |
| Y         | 90134          |
| Z         | 90464          |
| a         | 1447446        |
| b         | 50             |
| c         | 800            |
| d         | 12850          |
| e         | 12800          |
| f         | 204850         |
| g         | 205600         |
| h         | 3289650        |
| i         | 100            |
| j         | 1600           |
| k         | 25700          |
| l         | 25600          |
| m         | 409700         |
| n         | 411200         |
| o         | 6579300        |
| p         | 296            |
| q         | 4736           |
| r         | 1212712        |
| s         | 75776          |
| t         | 19398952       |
| u         | 19403392       |
| v         | 4967268648     |
| w         | 598            |
| x         | 9568           |
| y         | 2450006        |
| z         | 153088         |
| !         | 39191126       |
| "         | 39200096       |
| #         | 10035225174    |
| $         | 1298           |
| %         | 20768          |
| &         | 5317906        |
| '         | 332288         |
| (         | 85067026       |
| )         | 85086496       |
| *         | 21782144274    |
| +         | 4132           |
| ,         | 66112          |
| -         | 270798884      |
| .         | 1057792        |
| /         | 4332720164     |
| :         | 4332782144     |
| ;         | 17747075665956 |
| <         | 8264           |
| =         | 132224         |
| \>        | 541597768      |
| ?         | 2115584        |
| @         | 8665440328     |
| [         | 8665564288     |
| \         | 35494151331912 |
| ]         | 16534          |
| ^         | 264544         |
| _         | 1083588758     |
| `         | 4232704        |
| {         | 17337172118    |
| \|        | 17337420128    |
| }         | 71014072860822 |
| ~         | 33170          |
|           | 530720         |