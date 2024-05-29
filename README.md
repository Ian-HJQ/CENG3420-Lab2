# CENG3420-Lab2

## Lab 2-1: RISC-V RV32I Assembler

#### 1. Get the RV32I Assembler:

`$ git clone https://github.com/baichen318/ceng3420.git`

`$ cd ceng3420`

`$ git checkout lab2.1`

#### 2. Compile:

`$ make`

#### 3. Run the Assembler:

`$ ./asm benchmarks/isa.asm isa.bin` 

check the output machine code: isa.bin if you have implemented the assembler

#### Tasks:

Finish the RV32I assembler including 26+ instructions in asm.c as follows

- Pseudo instruction: la
- Integer Register-Immediate Instructions: slli, xori, srli, srai, ori, andi, lui
- Integer Register-Register Operations: sub, sll, xor, srl, sra, or, and
- Unconditional Jumps: jalr, jal
- Conditional Branches: bne, blt, bge
- Load and Store Instructions: lb, lh, lw, sb, sh, sw

These unimplemented codes are commented with `Lab2-1 assignment`

#### More Info: https://www.cse.cuhk.edu.hk/~byu/CENG3420/2022Spring/slides/lab2-1.pdf

## Lab 2-2: RISC-V RV32I Simulator

#### 1. Get the RV32I Simulator

`$ git clone https://github.com/baichen318/ceng3420.git`

`$ cd ceng3420`

`$ git checkout lab2.2`

#### 2. Compile

`$ make`

#### 3. Run the Simulator

`$ ./sim benchmarks/count10.bin`

the simulator can execute successfully if you have implemented it.

#### 4. Benchmarks

Verify your codes with these benchmarks (inside the benchmarks directory)
- isa.bin
- count10.bin
- swap.bin

#### 5. Verification

- isa.bin → a3 = -18/0xffffffee and MEMORY[0x84 + 16] = 0xffffffee
- count10.bin → t2 = 55/0x00000037
- swap.bin → NUM1 changes from 0xabcd to 0x1234 and NUM2 changes from 0x1234 to 0xabcd

#### Tasks:

Finish the RISCV LC simulator including 25 instructions in sim.c

- Integer Register-Immediate Instructions: slli, xori, srli, srai, ori, andi, lui
- Integer Register-Register Operations: sub, sll, xor, srl, sra, or, and
- Unconditional Jumps: jalr, jal
- Conditional Branches: bne, blt, bge
- Load and Store Instructions: lb, lh, lw, sb, sh, sw

These unimplemented codes are commented with `Lab2-2 assignment`

#### More Info: https://www.cse.cuhk.edu.hk/~byu/CENG3420/2022Spring/slides/lab2-2.pdf
