
### **1️⃣ Schematic Design (`schematic/`)**
- CMOS inverter circuit designed in **Cadence Virtuoso Schematic Editor**.
- Includes **PMOS and NMOS transistors**, power supply, and input/output terminals.
- Verified using **pre-layout simulations**.

### **2️⃣ Layout Design (`layout/`)**
- **Layout created in Virtuoso Layout Editor** following **DFM (Design for Manufacturing) guidelines**.
- Verified using **DRC (Design Rule Check)** and **LVS (Layout vs. Schematic) check**.
- Ensures correct transistor sizing and layout parasitics.

### **3️⃣ SPICE Netlist (`netlist/`)**
- The extracted **SPICE netlist (`netlist.sp`)** is used for post-layout simulations.
- Includes **parasitic components** to ensure accuracy.

---

## **Simulation Files (`invertor_sim/` Folder)**
The `invertor_sim` folder contains **simulation results and setup files** for the inverter.  

| **File Name**            | **Description** |
|-------------------------|----------------|
| `dc_analysis.tr0`       | DC transfer characteristics (input vs. output voltage) |
| `transient_analysis.tr0` | Transient response (waveforms of input and output signals) |
| `power_analysis.tr0`    | Power consumption during switching |
| `netlist.sp`            | SPICE netlist used for simulation |
| `sim_setup.scs`         | Cadence simulation setup file |
| `waveforms.png`         | Screenshot of simulated waveforms |

---

## **Simulation Results**
### **🔹 DC Analysis (Transfer Characteristics)**
- **Goal:** Analyze the inverter's switching threshold voltage.
- **Result:** Input vs. output voltage characteristics to determine the logic threshold.

### **🔹 Transient Analysis (Dynamic Behavior)**
- **Goal:** Study the inverter’s switching behavior when a pulse is applied.
- **Result:** Waveforms of input signal and corresponding output response.

### **🔹 Power Analysis**
- **Goal:** Measure **dynamic power consumption**.
- **Result:** Power dissipation due to charging/discharging of load capacitance.

---

## **How to Run the Simulation**
1. **Open Cadence Virtuoso** and navigate to the **"invertor"** folder.
2. Load the **schematic** in **Analog Design Environment (ADE-L or ADE-XL)**.
3. Open the **invertor_sim** folder and load the **simulation setup (`sim_setup.scs`)**.
4. **Run the simulation** and analyze results in **Virtuoso Waveform Viewer**.

---

## **Screenshots**
_Add screenshots of your schematic, layout, and simulation waveforms here._  
Example:
![Waveform Screenshot](docs/waveforms.png)

---

## **Future Improvements**
- Implement **power optimization techniques** to reduce dynamic/static power consumption.
- Extend the design to **complex combinational circuits** like NAND, NOR gates.
- Optimize transistor sizing for better performance.

---

## **License**
This project is open-source under the **MIT License**. You are free to use, modify, and share it.

---

### **📌 Uploading to GitHub**
Once you've saved this README as `README.md`, follow these steps to upload your project:

```sh

