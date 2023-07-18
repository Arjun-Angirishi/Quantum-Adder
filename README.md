# Building a basic Quantum Adder using Toffoli Gates

This repository contains implementation of Adder circuit using Toffoli Gates (CCNOT) amd CNOT gates. The Adder Circuits include single bit full adder and 4 bit full adder.
A project report is also added for discussion in greater detail.

## Problem Statement

Alice wishes to perform the addition of two 4-bit numbers using Quantum Circuits. Let those two numbers be a and b. In classical digital electronics, this is achieved using the full-adder circuit, which inputs the bits a_i,b_i and carry bit C_(i-1) and returns the sum bit S_i and carry bit C_i. Hence, the result of the computation would be as follows: Your task is to help Alice design a fully functional Quantum Adder using just CNOT and Toffoli Gates.

## Adder Circuit 

A single bit full adder circuit was made which takes 3 inputs, carry-in and the two bits and then it gives 2 outputs, 1 carry out bit and 1 S Sum bit.This single bit full adder was made using CX (CNOT) and CCX (Toffoli/CCNOT) gates. CX was mainly used as a XOR gate for evaluation of the S bit with toffoli gate used for carry-out calculations.

![Alt text](public\image.png)


Then as per the requirement of 4 bit adder, such 4 single bit adder circuit were cascaded to make the 4 bit adder. It requires 2 4-bit inputs A and B , along with 4 carry in quantum registers for interim calculations and give 5 bit output with a carry-out and 4 sum bits. 

![Alt text](public\image-1.png)
 
Simulations were done using QASM simulator which was run by 2048 shots in place of 1024 shots for more reliable results.

## Results 

Satisfactory Results were obtained for all the given test cases. 

## Made by
Arjun Angirishi <br>
20112023 <br>

#### For more details, Report added in the repository can be referred .