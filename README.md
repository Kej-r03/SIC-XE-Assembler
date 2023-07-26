SIC-XE-Assembler
====================

Author: Rishi Kejriwal

B.Tech C.S.E. 2nd Year

Indian Institute of Technology Roorkee.

This is the project for the Systems Software course, Spring 2023.

The requirment was to build a two-pass assembler for the SIC-XE machine in C/C++.
This is a SIC/XE Assembler with implementation of :
- [x] Basic Assembler.
  - [x] Input format free.
  - [x] Error handling.
- [x] Literals/org/equ support
- [ ] Program Blocks.
- [x] Control Sections.

Input :
- Freely formatted SIC/XE assembly program.

Output:
 - Object Code
 - List File
 - Symbol Table
 - Error Report (if neccessary)

Current Error:
 - Addressing mode.
 - Current Section name is not written in object record.


### Instructions :
```bash
# Clone this repository
git clone https://github.com/Kej-r03/SIC-XE-Assembler.git

# Go into repository
cd SIC-XE-Assembler/

# Compile Files into executable
g++ Main.cpp IO.cpp ExpressionEvaluator.cpp Pass1.cpp OpTab.cpp StringUtilities.cpp Parser.cpp OpCodeGenerator.cpp  Pass2.cpp Validate.cpp OperandHandler.cpp -o Assembler

# Now use assembler to convert your SIC-XE program :)
# Example
./Assembler Input/test_input.txt

#Output will be generated in listFile.txt and objectFile.txt
```