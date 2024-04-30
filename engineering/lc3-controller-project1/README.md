# LC-3 Project 1: Instruction Set Architecture
## Description
This project is inspired by NC State's ECE 745 course: ASIC Verification. The first of the course is designing and verifying a simple version of the LC-3 controller.

List of the simplifications compared to the full LC-3:
- Only operates on the following instructions: ADD, NOT, AND, LEA.
- All instructions take 5 clock cycles.
- Some of the inputs and outputs are not used: Mem_Control in the decode module; M_Data, Mem_contol_in, NZP, Mem_control_out in the execute module; psr in the writeback module.
- The processor is unpipelined and does not address pipeline issues like control and data dependence.

## Challenges
Some of the project specification had errors or were unclear. Thus, I could not simply follow all of the instructions, as some of them did not make sense. 
I conducted additional research in order to make sure I implemented all of the logic correctly. 

## Modules
