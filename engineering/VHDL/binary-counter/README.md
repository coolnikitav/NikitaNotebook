**Goal**: Design a replacement for a 74LS163 binary counter.

**Resources**: [74LS163 datasheet](https://d3c33hcgiwev3.cloudfront.net/ysffrwVNQz-H368FTfM_QQ_3f323db0b63c457d929fe7769bff873f_Motorola74LS16xA.pdf?Expires=1698796800&Signature=WLpcP1pc0Raqyz6AIun499bto8QEgwgr2wCncQMN-~zva8ah51jXFuCtP~v4VqTvlxYvdfpKvLXOQMX3aLmHTLK7ogE5ccCvUmxw-urvy3QHa7nz-P6UbkqRNd2BwFDQopcn7fsAMX~iHYErO~6-v7D7ROsEVVkzrRQqW1EwL6s_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

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

