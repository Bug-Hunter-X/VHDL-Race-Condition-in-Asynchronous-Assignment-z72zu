# VHDL Race Condition Example
This repository demonstrates a potential race condition in VHDL code when dealing with asynchronous signal assignments.

## Problem Description
The provided VHDL code attempts to copy data_in to data_out using a simple process. However, if the clock speed is high enough, the assignment of internal_data and data_out might not happen atomically. This leads to a race condition where the final value of data_out is uncertain.

## Solution
The solution incorporates proper synchronous signal assignments to eliminate the race condition and ensure reliable data transfer.

## Running the code
You can run the code using a suitable VHDL simulator, such as ModelSim or GHDL.  You might need to modify the testbench to observe the race condition.