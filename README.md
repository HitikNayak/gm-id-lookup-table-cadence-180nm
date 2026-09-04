# GM/ID Lookup Table Using Cadence Virtuoso – 180 nm CMOS

## 📌 Project Overview

This project focuses on the development of a **gm/ID-based lookup table for MOS transistor characterization and sizing** using **Cadence Virtuoso** and **180 nm CMOS technology**.

The generated lookup curves can be used to select a suitable transistor operating point and determine the required transistor width for analog CMOS circuit design.

---

## 🎯 Objective

To develop a **gm/ID lookup table** using 180 nm CMOS technology and analyze the relationship between:

* \(g_m/I_D\) and Overdrive Voltage \(V_{OV}\)
* \(g_m/I_D\) and Normalized Drain Current \(I_D/W\)

The lookup table can be used for **MOSFET bias-point selection and transistor sizing**.

---

## 🛠️ Tools and Technology

| Parameter              | Details          |
| ---------------------- | ---------------- |
| EDA Tool               | Cadence Virtuoso |
| Simulation Environment | Cadence ADE L    |
| CMOS Technology        | 180 nm           |
| Channel Length         | 180 nm           |
| DC Sweep Step          | 10 mV            |
| \(V_{DS}\) Sweep       | 0 V – 1.8 V      |
| Width \(W\) Sweep      | 400 nm – 2 µm    |
| Number of Sweep Points | 6                |

---

## 📐 Simulation Setup

A MOS transistor test circuit was designed in **Cadence Virtuoso** to generate the gm/ID lookup data.

### DC Analysis

The gate-source voltage \(V_{GS}\) was swept from:

**0 V to 1.8 V**

with a step size of:

**10 mV**

### Parametric Sweep

Two parameters were varied:

* Drain-source voltage \(V_{DS}\): 0 V to 1.8 V
* Transistor width \(W\): 400 nm to 2 µm

---

## 📊 Key Parameters

### Transconductance

The transconductance \(g_m\) represents how effectively the gate voltage controls the drain current.

### Overdrive Voltage

The overdrive voltage is defined as:

$$
V_{OV}=V_{GS}-V_{TH}
$$

where:

* V_{GS} = Gate-to-source voltage
* V_{TH} = Threshold voltage

### gm/ID

The ratio

$$
\frac{g_m}{I_D}
$$

is used as an important design parameter for selecting the operating region of a MOS transistor.

---

## 📈 Results

### 1. gm/ID vs VOV

The plot of \(g_m/I_D\) versus \(V_{OV}\) shows that **gm/ID decreases as overdrive voltage increases**.

This represents the transition from **weak inversion toward strong inversion**.

![gm/ID vs VOV](images/gm_id_vs_vov.png)

---

### 2. gm/ID vs ID/W

The plot of \(g_m/I_D\) against normalized drain current \(I_D/W\) provides a useful method for selecting the transistor operating point and determining the required transistor width.

![gm/ID vs ID/W](images/gm_id_vs_id_w.png)

---

## 🔍 Application

The generated lookup table can be used for:

* MOSFET bias-point selection
* Analog transistor sizing
* Selection of \(g_m/I_D\) operating point
* Estimation of transistor width
* Analog CMOS circuit design
* gm/ID-based design methodology

---

## 📁 Repository Structure

```text
gm-id-lookup-table-cadence-180nm/
│
├── README.md
│
├── schematic/
│   └── mos_test_circuit.png
│
├── simulation/
│   ├── ade_setup.png
│   └── parametric_sweep.png
│
├── results/
│   ├── gm_id_vs_vov.png
│   └── gm_id_vs_id_w.png
│
├── data/
│   └── lookup_table.xlsx
│
└── report/
    └── Assignment_2_CMOS.pdf
```

---

## 📌 Conclusion

The **gm/ID lookup table** was successfully generated using **Cadence Virtuoso with 180 nm CMOS technology**.

The simulations were performed by varying \(V_{DS}\) and transistor width while sweeping \(V_{GS}\). The resulting \(g_m/I_D\) versus \(V_{OV}\) and \(g_m/I_D\) versus \(I_D/W\) curves provide useful information for selecting a suitable MOS transistor bias point and determining the required transistor width for analog circuit design.

---

## 👨‍💻 Author

**Hitik Kumar Nayak**

M.Tech – Microelectronics and VLSI
IIT Bhilai

### Skills Demonstrated

`Cadence Virtuoso` · `Cadence ADE L` · `CMOS 180nm` · `Analog IC Design` · `MOSFET Characterization` · `gm/ID Methodology` · `Transistor Sizing`

---

## 📚 Project Type

**Academic / VLSI Design Assignment**

**Focus:** Analog CMOS Design and MOSFET Characterization
