# EE-329 A1 – STM32L4 GPIO Timing & Instrumentation Demo

This project demonstrates **low-level GPIO control and timing instrumentation** on an STM32L4 microcontroller.  
It combines STM32 HAL initialization with direct register access to achieve precise performance measurement in embedded systems.

---

## 🔹 Project Overview
- **GPIO strobe timing:**  
  - PC0 toggled around a function call to mark total execution time  
  - PC1 toggled inside the function to measure the duration of a `sin()` computation  
- **Low-level register programming:**  
  - Manual setup of GPIOC pins (PC0–PC3) as push-pull outputs at very high speed  
- **4-bit digital output demo (optional):**  
  - Binary counter across PC0–PC3 for LEDs or a logic analyzer  
- **Hybrid HAL + bare-metal approach:**  
  - HAL used for system setup, with direct register writes for performance-critical I/O

---

## 🛠️ Skills Demonstrated
- Embedded C programming for STM32
- Precise latency measurement with GPIO strobes
- Register-level microcontroller programming
- Integration of math library functions (`sin()`) into real-time code
- GitHub-ready repo organization with `.gitignore` and documentation

---

## 🚀 Getting Started
1. Clone this repository or [download as a zip](../../archive/refs/heads/main.zip).
2. Open in **STM32CubeIDE** (or your preferred IDE).
3. Build and flash to an STM32L4 target board.
4. Use an oscilloscope or logic analyzer on PC0/PC1 to observe timing behavior.

---

## 📂 Repository Structure
```
.
├── main.c          # Application code
├── main.h          # Header definitions & macros
├── .gitignore      # Ignore build artifacts/IDE files
└── README.md       # Project description (this file)
```

---

## 📈 Learning Outcomes
This assignment highlights:
- Writing **clean, modular embedded code**
- Using GPIO as a **timing probe** for function profiling
- Balancing **HAL convenience with direct register efficiency**
- Preparing and presenting projects in a **professional GitHub format**

---

## 📝 Notes
- Tested on STM32L4 series microcontroller
- Build products (`.elf`, `.bin`, etc.) and IDE metadata have been excluded to keep the repo clean
- The optional binary counter loop can be re-enabled for lab demonstrations

---

👤 **Author:** Nathan Heil  
📅 **Course:** EE-329 (Embedded Systems)  
