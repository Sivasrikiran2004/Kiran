## Task-2  
R-type instruction
<pre>
  These are used for operations involving only registers without immediate values.  
  Typically include arithmetic,logical and comparison instructions. 
</pre>
Format of R-type instruction
<pre>
    31      25 24    20 19    15 14    12 11     7 6        0  
    |  funct7 |  rs2   |  rs1   | funct3 |   rd   |  opcode | 
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]
- rd: It is the destination register which stores the destination address.  
          It is of 5 bits [11:7]  
- funct3: It specifies the function code for the operation.  
          It is of 3 bits [14:12]  
- rs1: It specifies the source register 1.  
          It is of 5 bits [19:15]  
- rs2: It specifies the source register 2.  
          It is of 5 bits [19:15]  
- funct7: It specifies the function for the operation.  
          It is of 7 bits [31:25]  
</pre>
  
I-type instruction  
<pre>
  These are used for operations involving immediate values along with registers.  
  Typically include arithmetic,logical and data transfer operations.  
</pre>
Format of I-type instruction
<pre>
    31      20 19    15 14    12 11     7 6       0
    |   imm   |  rs1   |  funct3|   rd   | opcode |
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]
- rd: It is the destination register which stores the destination address.  
          It is of 5 bits [11:7]
- funct3: It specifies the function code for the operation.  
          It is of 3 bits [14:12]
- rs1: It specifies the source register 1.  
          It is of 5 bits [19:15]
- imm: It specifies the immediate value.
          It is of 12 bits [31:20]  
</pre>
S-type instruction
<pre>
  These are used for storing data from a register into memory.
</pre>  
Format of S-type instruction  
<pre>
    31      25 24    20 19    15 14    12 11     7 6       0
    |imm[11:5]|  rs2   |  rs1   |  funct3|imm[4:0]| opcode |
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]  
- rs1,rs2: These fields contain register numbers  
           It is of 5 bits each  
- funct3: It specifies the function code for the operation.  
          It is of 3 bits [14:12]  
- imm : It specifies the immediate value.
        It is of 12 bits
</pre>
B-type instruction
<pre>
  These instructions are used for conditional branching based on a condition evaluated from comparing two register values.
</pre>
Format of B-type instruction
<pre>
    31        30       25 24    20 19    15 14    12 11       8        7 6       0
    |  imm[12]| imm[10:5]|  rs2   |  rs1   |  funct3| imm[4:1]| imm[11] | opcode |
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]  
- rs1,rs2: These fields contain register numbers  
           It is of 5 bits each  
- funct3: It specifies the function code for the operation.  
          It is of 3 bits [14:12]  
- imm : It specifies the immediate value.
        It is of 12 bits
</pre>
U-type instruction 
<pre>
  These instructions are used for operations with immediate values that are wider than 12 bits.
</pre>
Format of U-type instruction
<pre>
    31                   12 11     7 6       0
    | imm[31:12]           |  rd    | opcode |
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]  
- rd: It is the destination register which stores the destination address.  
      It is of 5 bits [11:7]  
- imm: It specifies immediate value
       It is of 20 bits [31:12]  
</pre>
J-type instruction 
<pre>
  These instructions are used for unconditional jumps.
</pre>
Format of J-type instruction
<pre>
   31     30 29       21 20     19 18        12 11     7 6       0
   |imm[20] | imm[10:1] | imm[11] | imm[19:12] |    rd  | opcode |
</pre>
<pre>
- opcode: It is a part of instruction which specifies the operation to be performed.  
          It is of 7 bits [6:0]  
- rd: It is the destination register which stores the destination address.  
      It is of 5 bits [11:7]  
- imm: It specifies immediate value
       It is of 20 bits 
</pre>
Examples
<pre>
  1.add r7,r1,r2
</pre>
