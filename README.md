This project is an Intel x86 assembler written in C. The assembler translates x86 assembly code into machine code (OBJ2 binary format) that can be run on an emulated Intel machine with a graphics card. The project includes functionality to handle data declarations, instruction encoding, and the generation of segment descriptors for memory segmentation.

Features
Assembly to Machine Code Translation: Converts Intel x86 assembly instructions into 32-bit machine code.
Data Segment Encoding: Supports encoding of .data and .data? sections into binary format.
Instruction Encoding: Encodes instructions based on a custom 32-bit binary method, ensuring compatibility with the target emulator.
Segment Descriptors: Generates segment descriptors for memory layout (header, data, code, and stack segments).
Symbol Table Generation: Maintains a symbol table for variable offsets and instruction locations.
Error Handling: Basic error reporting for syntax issues and incorrect file handling.

Files
assembler.c: Handles parsing of the assembly file, encoding, and writing the machine code to the output file.
encode.c/h: Handles instruction encoding into machine code.
test.c/h: Encodes and processes data declarations into binary format.
symbol_table.txt: Stores the generated symbol table for reference.

