Team Members:
Ben 
Oliver
Kai

Input is: R1

output is: R3 (upper), R2 (lower)

HeraDP Code
CBON()
SET(R1,24)
SET(R2,1)
SET(R4,1)
LABEL(LOOP)
OPCODE(0x2A21) // R3,R2 += R5,R4
MOVE(R3,R5)
MOVE(R2,R4)
MOVE(R5,R7)
MOVE(R4,R6)
DEC(R1,1)
CMP(R1,R0)
BNZ(LOOP)

Machine Code:
 3160
  e118
  f100
  e201
  f200
  e401
  f400
  2a21
  9350
  9240
  9570
  9460
  31c0
  3068
  b010
  eb07
  fb00
  190b
