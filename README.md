# 🚀 RV32I Assembler in Python

<div align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![RISC-V](https://img.shields.io/badge/RISC--V-RV32I-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Architecture](https://img.shields.io/badge/Computer-Architecture-orange?style=for-the-badge)

### ⚡ Python-based RISC-V RV32I assembler  
Convert assembly instructions into **32-bit binary machine code** with label handling, syntax validation, and detailed error reporting.

</div>

---

# 📌 Overview

This project implements a **RISC-V RV32I Assembler** in Python capable of translating assembly instructions into executable binary machine code.

The assembler supports all major RV32I instruction formats, performs syntax and operand validation, resolves labels and branch offsets, and generates accurate machine code suitable for architecture simulators and educational projects.

---

# ✨ Features

✅ Supports multiple RV32I instruction formats  
✅ Converts assembly code to 32-bit binary machine code  
✅ Handles labels and branch calculations  
✅ Performs syntax and register validation  
✅ Detects invalid instructions and immediates  
✅ Provides detailed line-number-based error messages  
✅ Designed for simulator integration and automated testing  

---

# 🧠 Supported Instruction Types

| Type | Supported Instructions |
|------|-------------------------|
| 🔹 **R-Type** | `add`, `sub`, `sll`, `slt`, `sltu`, `xor`, `srl`, `or`, `and` |
| 🔹 **I-Type** | `lw`, `addi`, `sltiu`, `jalr` |
| 🔹 **S-Type** | `sw` |
| 🔹 **B-Type** | `beq`, `bne`, `blt`, `bge`, `bltu`, `bgeu` |
| 🔹 **U-Type** | `lui`, `auipc` |
| 🔹 **J-Type** | `jal` |

---

# 📂 Project Structure

```bash
📦 RV32I-Assembler
 ┣ 📜 assembler.py
 ┣ 📜 input.asm
 ┣ 📜 output.txt
 ┗ 📜 README.md
```

---

# ⚙️ How to Run

## ▶️ Command

```bash
python assembler.py input.asm output.txt
```

---

# 📝 Example

## 📥 Input (`input.asm`)

```assembly
addi x1, x0, 10
addi x2, x0, 20
add x3, x1, x2
beq zero, zero, 0
```

---

## 📤 Output (`output.txt`)

```text
00000000101000000000000010010011
00000001010000000000000100010011
00000000001000001000000110110011
00000000000000000000000001100011
```

---

# 🛡️ Error Handling

The assembler detects and reports:

| ❌ Error Type | 📌 Description |
|---|---|
| Invalid Instruction | Unsupported opcode/instruction |
| Invalid Register | Unknown register name |
| Syntax Error | Incorrect instruction formatting |
| Undefined Label | Branch/jump label not found |
| Immediate Overflow | Immediate value out of range |
| Invalid Arguments | Incorrect number of operands |
| Invalid Branch Offset | Non-aligned branch immediate |
| Missing Virtual Halt | Required halt instruction missing |

---

# 🏗️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Core implementation |
| 🔍 Regular Expressions (`re`) | Parsing and validation |
| 📂 File Handling | Input/output processing |

---

# 🎯 Applications

- 📘 Computer Architecture coursework
- 🖥️ RISC-V ISA learning
- ⚙️ Assembly-to-machine-code translation
- 🧪 Architecture simulator integration
- 📚 Educational and academic projects

---

# 🚧 Future Improvements

- 🔸 Hexadecimal output support
- 🔸 Pseudo-instruction support
- 🔸 ELF file generation
- 🔸 Pipeline simulation integration
- 🔸 Interactive debugging utilities

---

# 👨‍💻 Author
## this is a group project with 4 member 
## ** i am Prabhav Agrawal**

🎓 First-Year B.Tech Student  
📚 Computer Science and Applied Mathematics  

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star!

</div>
