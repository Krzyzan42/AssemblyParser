# AssemblyParser

Assembly parser in assembly. It recognizes some basic commands like 'ADD', 'MULT' or 'JR', validates them on enter and stores on stack, so at the end of the program they get printed out in reverse order. 

## Example
![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/1f65bfd0-2525-4e92-a67b-133ebb522508)
![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/e05947dc-7972-463d-87e0-bc4a201fe25f)

## Possible instructions
There are registers, labels and immediates. Registers are from range $0 - $31, labels can be composed only of letters (both lowercase and uppercase), immediates are just numbers (negatives are allowed). If instruction argument doesn't match expected type, user is asked, to type instruction again

- ADD `register` `register` `register`
- ADDI `register` `register` `immediate`
- J `label`
- NOOP
- MULT `register` `register` `register`
- JR `register`
- JAL `label`

## Invalid instructions
Adding this section just because I'm proud of that
<hr>
Register number too big

![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/06bd6997-8a8f-49b5-a602-83b59d621623)
<hr>
Invalid number of arguments

![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/fa69c558-7fae-4361-b389-7cc68298d29b)
<hr>
Illegal character in label

![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/3de8e525-370d-465b-92fa-982ac9790a28)
<hr>
Immediate secretly isn't a number

![image](https://github.com/Krzyzan42/AssemblyParser/assets/100627976/cfb510a7-5d05-4a0e-8f75-9a9f524aa62a)

