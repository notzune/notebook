ZPL is a print language used by many label printers. a print language is a set of commands that can be used to draw elements like text, shapes, barcodes and images, combine these elements, and finally print them; formally it is a [[Page description language (PDL)|page description language]] from Zebra Technologies used primarily for labeling applications. 

the language commands always start with a caret ('^') or a tilde ('~'). each format has to start with the  command `^XA` and end with `^XZ`.

for instance the font size is sent to the printer with the `^ADN,n,m` command. where `n` and `m` are [[Integer|integers]] denoting the font size and spacing characteristics. 

`^ADN,18,10` is the smallest size and `^ADN,180,100` the largest.

imagine that you want to print a label containing a product name, a barcode for a SKU number, and a box around it all., below is an example of a ZPL label template that does just this. 

```zpl
^XA
^FO50,60^A0,40^FDWorld's Best Griddle^FS
^FO60,120^BY3^BCN,60,,,,A^FD1234ABC^FS
^FO25,25^GB380,200,2^FS
^XZ
```

