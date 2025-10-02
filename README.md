⚙️ 4-BIT ARITHMETIC LOGIC UNIT (ALU) DESIGN

Introduction

This project demonstrates the ability to design digital systems from the lowest level. We successfully designed and implemented a 4-bit Arithmetic Logic Unit (ALU)—a core component of a Central Processing Unit (CPU)—built entirely from fundamental logic gates.

    Functions: Addition, Subtraction, Multiplication (minimal), and XOR.

    Basis: Digital Circuit Theory, Combinational Design.

    Core Components: AND, OR, and NOT logic gates only.

🎯 Project Goal

The primary goal of this project was to master and apply core digital logic principles to construct a complex functional block using only the most basic modules:

    Gate-Level Design: Converting complex Boolean expressions and logic into electronic circuits using only basic gates (AND, OR, NOT).

    Subtraction Implementation: Understanding and implementing subtraction using the two's complement method, illustrating how computers handle negative numbers and subtraction operations.

    Integration and Control: Building a system of MUXes and control logic to correctly select and output one of the four distinct functions.

🏛️ Design Architecture

The ALU is structured into functional units, each built from AND, OR, and NOT gates, and then combined using a Multiplexer (MUX).

1. Inputs, Outputs, and Control

    Inputs A, B: 4-bit. The two operands A and B.

    Control Signal (S1​S0​): 2-bit. Selects one of the 4 functions (e.g., 00 for Add, 01 for Subtract, etc.).

    Result R: 6-bit (R5​…R0​). The output result. 6 bits are used to correctly represent the full result of multiplying two 4-bit numbers (up to 15×15=225).

2. Functional Units

    Arithmetic Unit (Add/Subtract): Uses 4 cascaded Full Adders (Ripple-Carry). Subtraction is implemented using two's complement (inverting B using NOT gates and setting the Carry-in to 1).

    Logic Unit (XOR): The 4-bit XOR function is constructed solely from a combination of AND, OR, and NOT gates.

    Multiplication Unit: A combinational circuit designed to perform minimal 4-bit multiplication.

    Multiplexer (MUX 4-to-1): Also constructed from basic gates, it uses the S1​S0​ signal to select the correct result from the functional units and pass it to the final output R.

✨ Project Highlights

    Basic Gate Mastery: The project demonstrates the ability to build complex functional blocks from the foundational AND, OR, NOT gates, validating expertise in gate-level design.

    Flexible Word Length Handling: Designing the output to be 6 bits (instead of a standard 4 bits) shows an understanding of data overflow and the ability to correctly manage variable word lengths in computer architecture.

    Core CPU Modeling: Successfully modeling the fundamental operational mechanism of an ALU provides a solid foundation for more complex CPU and microprocessor design projects.
