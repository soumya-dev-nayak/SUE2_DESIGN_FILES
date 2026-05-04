# 🧠 SUE2 Design Files Repository

Welcome! This repository contains schematic design files, lab work, and personal projects created using **SUE2 (Schematic User Environment 2)** along with simulation workflows.

---

# 🚀 1. Prerequisites

Before using this repository, make sure you have the following installed on your system:

- Linux / WSL (recommended)
- Git
- SUE2
- (Optional) ngspice for simulation

---

# 🛠️ 2. Installing SUE2 (Ubuntu / WSL)

## Step 1: Install dependencies
```bash
sudo apt update
sudo apt install git build-essential tcl tk
```

## Step 2: Clone SUE2
```bash
git clone https://github.com/RTimothyEdwards/sue2.git
cd sue2
```

## Step 3: Build SUE2
```bash
./configure
make
```

## Step 4: Run SUE2
```bash
./sue2
```

(Optional) Add to PATH:
```bash
sudo ln -s ~/sue2/sue2 /usr/local/bin/sue2
```

Now you can launch it using:
```bash
sue2
```

---

# 📥 3. Clone This Repository

```bash
git clone https://github.com/soumya-dev-nayak/SUE2_DESIGN_FILES.git
cd SUE2_DESIGN_FILES
```

---

# 📂 4. Copy Files into SUE2 Library

SUE2 uses a library folder (usually inside CppSim):

```bash
C:\CppSim\SueLib
```

## Copy repository folders:

### For Linux/WSL:
```bash
cp -r SOUMYA_DEV_VLSI_LAB_FILES /mnt/c/CppSim/SueLib/
cp -r MY_FILES /mnt/c/CppSim/SueLib/
```

### For Windows (PowerShell):
```powershell
xcopy SOUMYA_DEV_VLSI_LAB_FILES C:\CppSim\SueLib\ /E /I
xcopy MY_FILES C:\CppSim\SueLib\ /E /I
```

---

# 🧩 5. Open Designs in SUE2

1. Launch SUE2:
```bash
sue2
```

2. In SUE2:
- Go to **Library Browser**
- Locate:
  - `SOUMYA_DEV_VLSI_LAB_FILES`
  - `MY_FILES`
- Open any schematic

---

# ⚡ 6. Running Simulations

## Option 1: Using ngspice

Export netlist from SUE2 and run:
```bash
ngspice filename.sp
```

## Option 2: Using CppSim tools

- Use built-in simulation environment
- Configure paths if required

---

# 📁 7. Repository Structure

```
SUE2_DESIGN_FILES/
 ├── SOUMYA_DEV_VLSI_LAB_FILES/   # Lab experiments
 ├── MY_FILES/                    # Personal designs
 └── README.md
```

---

# ⚠️ 8. Important Notes

- Do NOT move files randomly inside SueLib
- Keep folder names unchanged
- Some designs may depend on specific libraries
- Simulation files (.raw, .log) are not included

---

# 🧪 9. Example Workflow

1. Open SUE2
2. Load a design from `MY_FILES`
3. Modify schematic
4. Export netlist
5. Run in ngspice

---

# 🧠 10. Tips for Beginners

- Start with simple circuits (RC, amplifier)
- Understand netlist generation
- Use consistent naming
- Keep backups using Git

---

# 🤝 Contributions

Feel free to fork and improve designs.

---

# ⭐ Credits

Created and maintained by Soumya Dev Nayak

---

Happy Designing! 🚀
