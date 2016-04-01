
The program does not print anything out, but disassembling the code into pseudo c code
tells us that things are going on in the background. If we set a break point at 0x08048e9e,
we can slowly print out the various characters of the flag contained in %eax. Turning the ascii values
into characters, we can reconstruct the flag
<br>
flag{l0k_hype_1s_too_r3al}
<br>The solution lies in the stack of the program.
