**Goal**: Design a replacement for a 74LS163 binary counter.

**Resources**: [74LS163 datasheet](https://datasheetspdf.com/pdf-file/375457/FairchildSemiconductor/74LS163A/1)

**Plan**:
1. Determine inputs and outputs.
2. Create entity block.
3. Determine the logic (how inputs and outputs interact).
4. Create the architecture block.
5. Simulate to verify that the design is working.
6. Make edits if the design is not working.

**Design**:

Inputs: CP (clock), SR (synchronous reset, active low), P (parallel input), PE (parallel load), CEP (count enable parallel input), CET (count enable trickle input).

Outputs: Q, TC (terminal count).

