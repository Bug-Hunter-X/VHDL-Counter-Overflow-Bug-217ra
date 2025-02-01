# VHDL Counter Overflow Bug
This repository demonstrates a potential overflow issue in a simple VHDL counter. The `buggy_counter.vhdl` file contains the buggy code, while `fixed_counter.vhdl` provides a corrected version.

## Bug Description
The original counter is supposed to count from 0 to 15. However, if not properly initialized or if the simulation/synthesis tools handle the overflow condition unexpectedly, the counter may behave unexpectedly or produce incorrect results.  The issue is subtle and might only show up under specific conditions.

## Solution
The `fixed_counter.vhdl` uses more robust handling.  The solution ensures that the count is always within the desired range.  It provides explicit checks and handling for the maximum count value, preventing unexpected behavior.