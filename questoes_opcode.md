> Projete um opcode de expansão para permitir
que todos os seguintes sejam codificados em uma instrução de 36 bits:<br>
-> 7 instruções com dois endereços de 15 bits e um número de reigstrador de 3 bits <br>
-> 500 instruções um endereço de 15 bits e um número de registrador de 3 bits
-> 40 instruções sem nenhum endereço nem registrador

- Solução:

7 instruções com dois endereços de 15 bits e um número de registrador de 3 bits

P: 0000 00XX XXXX XXXX XXXX XXXX XXXX XXXX XXXX	

U: 0001 10XX XXXX XXXX XXXX XXXX XXXX XXXX XXXX

0000 0000 <br>
0000 0110 + <br>
___________ <br>
0000 0110 <br>

500 instruções com um endereço de 15 bits e um número de registrador de 3 bits

P: 0000 0111 0000 0000 0000 000X XXXX XXXX XXXX

Somando com 499<sub>DEC</sub> => 0001 1111 0011<sub>BIN</sub>:

U: 0000 0111 0000 0001 1110 011X


