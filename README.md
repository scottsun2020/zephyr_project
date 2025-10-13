## Starter Sample
https://docs.zephyrproject.org/latest/develop/getting_started/index.html

---

## 🧩 Project Overview

**Goal:** Run and manage embedded firmware on Nordic’s nRF52840 Development Kit using Zephyr RTOS.  
**Current milestone:** ✅ LED Blinky app running successfully via `west flash -r nrfutil`.

### Features
- Built on **Zephyr RTOS 4.2.99**
- Flashed with **nRF Util 8.1.1**
- Debugged with **SEGGER J-Link 8.74a**
- Managed via **`west` + CMake + Ninja**
- Works on **Ubuntu 24.04** environment

---

## 🧰 Development Environment Setup

### 1. Install Zephyr SDK and Tools
```bash
pip install west
west init ~/zephyrproject
cd ~/zephyrproject
west update
west zephyr-export
pip install -r zephyr/scripts/requirements.txt

```


### 2. Build Blinky Sample

```
cd ~/zephyrproject/zephyr
west build -p always -b <your-board-name> samples/basic/blinky
west flash -r nrfutil
```

![ezgif-4421fff72fb6c1](https://github.com/user-attachments/assets/6725ccf9-7a67-470c-9693-cc30709aaebe)
