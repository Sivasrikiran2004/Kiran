# Kiran  
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
          It is of 3 bits [12:14]  
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
          It is of 3 bits [12:14]
- rs1: It specifies the source register 1.  
          It is of 5 bits [19:15]
- imm: It specifies the immediate value.
          It is of 12 bits [31:20]  
</pre>
