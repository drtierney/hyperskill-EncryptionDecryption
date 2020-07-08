# hyperskill-EncryptionDecyption
Developing a command line application which can encrypt/decrypt strings using various encryption algorithms.  
https://hyperskill.org/projects/46

<img src="https://github.com/drtierney/hyperskill-EncryptionDecryption/blob/master/EncryptionDecryption.gif" width="800" height="500" />

## Syntax

| Arg | Valuelist | Comment
| --- | --------- | ------- |
| -mode | enc<br>dec | Required<br>Choose to encode or decode input|
| -data | `<String>` | Requires at least one (-data OR -in)<br>input text<br>If both -data and -in exist, -data is prioritised|
| -alg  | shift<br>unicode | Required<br>Choose algorithm to use|
| -key  | `<Integer>`| Not Required<br>default is 0 (no change to input)|
| -in   | `<String>` | Requires at least one (-data OR -in)<br>input filepath<br>If both -data and -in exist, -data is prioritised|
| -out  | `<String>` | Not Required<br>output filepath<br>if omitted outputs to console window|

```
EncryptionDecryption.jar -mode enc -key 5 -data "Hello World" -alg unicode
```
```
EncryptionDecryption.jar -mode dec -key 7 -data "Encryption Decryption -alg shift -out "D:\Temp\output.txt"
```
```
EncryptionDecryption.jar -mode dec -key 10 -in "D:\temp\input.txt" -alg shift
```

## Stages

**Stage #1 Encrypted**  
Learn to input the data and encrypt it, replacing the letters.

**Stage #2 Knowledge is key**  
Learn to encrypt messages with a numeric key, using the Caesar cypher. 

**Stage #3 Decrypted!**  
Encrypting a message is only half of the deal: now learn to decrypt it as well, using a standard Unicode table.

**Stage #4 I Command you**  
Practice working with the command line, using it for passing the mode, the key and the string.

**Stage #5 X-files**  
Work with files; learn to store your data in a file.

**Stage #6 Choices, Choices**  
Add the possibility to choose a specific encryption algorithm: Ceasar or Unicode.
