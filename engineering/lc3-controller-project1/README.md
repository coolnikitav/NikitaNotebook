# LC-3 Project 1: Instruction Set Architecture
## Description
This project is inspired by NC State's ECE 745 course: ASIC Verification. The first of the course is designing and verifying a simple version of the LC-3 controller.

List of the simplifications compared to the full LC-3:
- Only operates on the following instructions: ADD, NOT, AND, LEA.
- All instructions take 5 clock cycles.
- Some of the inputs and outputs are not used: Mem_Control in the decode module; M_Data, Mem_contol_in, NZP, Mem_control_out in the execute module; psr in the writeback module.
- The processor is unpipelined and does not address pipeline issues like control and data dependence.

## Modules
The LC-3 Controller consists of 4 modules: Fetch, Decoce, Execute, Writeback. Components were designed and verified individually. Then they were combined them into a main controller design and it was verified that all 5 stages of the pipeline work cohesively. 

Each of the folders have specifications, intended module behavior, schematics, design files, testbench files, and simulation outputs:
- [Fetch](https://github.com/coolnikitav/nikitas-notebook/tree/5ba684eed46259b160b7792295dfdfa551b46786/engineering/lc3-controller-project1/fetch)
- [Decode](https://github.com/coolnikitav/nikitas-notebook/tree/5ba684eed46259b160b7792295dfdfa551b46786/engineering/lc3-controller-project1/decode)
- [Execute](https://github.com/coolnikitav/nikitas-notebook/tree/5ba684eed46259b160b7792295dfdfa551b46786/engineering/lc3-controller-project1/execute)
- [Writeback](https://github.com/coolnikitav/nikitas-notebook/tree/5ba684eed46259b160b7792295dfdfa551b46786/engineering/lc3-controller-project1/writeback)
- [Controller - Combines the 4 modules into a full processor](https://github.com/coolnikitav/nikitas-notebook/tree/5ba684eed46259b160b7792295dfdfa551b46786/engineering/lc3-controller-project1/controller)

## Skills
- Testbenches we written in SystemVerilog.
- Testbenches utilized:
  - Random stimulus
  - Functional coverage: interface, transaction, generator, driver, monitor, scoreboard, environment
  - Assertion-based verification methodologies
- The design files were written in Verilog.
- Required understanding of pipelines and uniprocessor architecture.

## Challenges
Some of the project specification had errors or were unclear. Thus, I could not simply follow all of the instructions, as some of them did not make sense. 
I conducted additional research in order to make sure I implemented all of the logic correctly. 
