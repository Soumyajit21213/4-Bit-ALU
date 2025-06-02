# 4-bit CMOS ALU – Built from Scratch Using Transistors

Welcome to my project where I’ve designed and simulated a **4-bit Arithmetic Logic Unit (ALU)** using only **CMOS-based logic gates**. This ALU performs essential binary operations at the transistor level, offering a hands-on insight into how digital computation works under the hood.

---

## Features
Built entirely from **CMOS logic (PMOS + NMOS transistors)** 
Zero loading effect – **high-efficiency logic gate behavior**  
Modular design: Gates → Operations → ALU  
8 Supported Operations via OpCode selector  
Designed and simulated in **LTspice**

---

## Supported Operations

The ALU can perform the following 8 operations:

| OP Code | Operation     | Description                   |
|--------:|----------------|-------------------------------|
| `000`   | AND           | Bitwise A AND B              |
| `001`   | OR            | Bitwise A OR B               |
| `010`   | XOR           | Bitwise A XOR B              |
| `011`   | NOT A         | Bitwise NOT of A             |
| `100`   | ADD           | A + B                        |
| `101`   | SUB           | A - B                        |
| `110`   | INCREMENT     | A + 1                        |
| `111`   | LEFT SHIFT    | A << 1 (Logical Left Shift)  |

Each operation result is displayed for **2 seconds sequentially** in the simulation. You can also manually select any operation by changing the **OpCode (3-bit)** value.

---

## Project Structure
├── Gates/ # CMOS implementations of basic logic gates
├── Operations/ # Circuits for each of the 8 ALU operations
├── Mux/ # 8:1 digital multiplexer (one for each output bit)
├── ALU_Final/ # Fully integrated 4-bit ALU circuit
├── Screenshots/ # Sample waveforms and output images
└── README.md # Project overview and instructions



---

## How to Simulate

1. Open the `.asc` files using **LTspice**.
2. Set your 4-bit inputs A and B (e.g., A = `1001`, B = `0101`).
3. OpCode cycles automatically every 2 seconds to show each operation.
4. Alternatively, fix OpCode to a specific value to lock a single operation.

---

## Highlights & Learnings

- Designed CMOS logic gates from scratch (AND, OR, NOT, XOR, etc.)
- Built a full 4-bit **full adder**, **subtractor**, and **mux** at the transistor level
- Developed compact and efficient implementations of digital operations
- Learned how **gate-level logic** composes higher-level components like ALUs
- Explored the advantages of CMOS: **zero static power loss, no loading effect**

---

## Example

Inputs:  
- A = `1001`  
- B = `0101`  

Output results for each OpCode operation are visible on the waveform simulation.  
Feel free to test with your own inputs and OpCodes!

---

##  About Me

👤 **Soumyajit Samanta**  
Electronics enthusiast | Digital design explorer | Embedded systems learner

🔗 [LinkedIn](https://www.linkedin.com/in/your-profile/) *(Insert your LinkedIn URL)*
Mail ID : 23je0964@iitism.ac.in

---

Feel free to fork this repo, test the design, or reach out if you have ideas to collaborate!
