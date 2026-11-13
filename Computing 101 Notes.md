# Computing 101 Notes**


## Registers

They live in the CPU.

Data goes from the system memory to caches and then into registers, where it is manipulated/interacted with by the CPU for operations etc. It's the size of the register e.g. amd64, which means it can hold 64 bits or 8 bytes in each register.

The registers are actually pretty limited and apparently have individual names and certain purposes. **Rax** is the one used to store data to be moved and rdi, rsi etc are commonly used as parameters to a system call (syscall).

Also, numbers by themselves are treated as values, but inside of [] they turn into memory address. This works even if you put a number, 12345 for example, into rax and then do "mov rdi, [rax]" it will turn the value in rax into the address [12345]

**Turn Assembly file into program
as program.o program.s
ld -o program program.o
