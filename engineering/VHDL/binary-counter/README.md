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

Inputs: CP (clock), SR (synchronous reset, active low), P[3:0] (parallel input), PE (parallel load), CEP (count enable parallel input), CET (count enable trickle input).

Outputs: Q[3:0], TC (terminal count).

Schematic:

![image](https://github.com/coolnikitav/nikitas-notebook/assets/30304422/612ed0cf-f283-4ed0-854c-b1ca25845710)

Logic:

If PE = 0 => Q = P

If SR = PE = CET = CEP = 1 => Count

If PE = 1 and (CET = 0 or CEP = 0) => No change (hold)

If CET = Q3 = Q2 = Q1 = Q0 = 1 => TC = 1 (reached highest count)

If SR = 0 => Q3 = Q2 = Q1 = Q0 = 0 (clear)
