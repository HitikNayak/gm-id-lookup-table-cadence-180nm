# MOS Transistor Test Circuit

## Overview

This folder contains the **MOS transistor test circuit** designed in **Cadence Virtuoso** for generating the \(g_m/I_D\) lookup table using **180 nm CMOS technology**.

The schematic is used to obtain the MOS transistor characteristics required for calculating and plotting:

$$
\frac{g_m}{I_D}\ \text{vs.}\ V_{OV}
$$

and

$$
\frac{g_m}{I_D}\ \text{vs.}\ \frac{I_D}{W}
$$

## Technology

* **Technology:** 180 nm CMOS
* **Channel Length:** \(L = 180\,\text{nm}\)
* **Simulation Tool:** Cadence Virtuoso
* **Analysis:** DC Analysis and Parametric Sweep

## Purpose of the Circuit

The MOS transistor test circuit is used to extract the electrical parameters required for the \(g_m/I_D\) lookup-table methodology.

The important parameters obtained from the simulation include:

* Gate-to-source voltage \(V_{GS}\)
* Drain-to-source voltage \(V_{DS}\)
* Drain current \(I_D\)
* Transconductance \(g_m\)
* Overdrive voltage \(V_{OV}\)
* \(g_m/I_D\)
* Normalized drain current \(I_D/W\)

## Simulation Conditions

The gate-to-source voltage is swept from:

$$
V_{GS}=0\text{ V to }1.8\text{ V}
$$

with a step size of:

$$
\Delta V_{GS}=10\text{ mV}
$$

The parametric variables are:

$$
V_{DS}=0\text{ V to }1.8\text{ V}
$$

and

$$
W=400\text{ nm to }2\,\mu\text{m}
$$

## Schematic

The schematic shown in this folder is the MOS transistor test circuit used for the lookup-table generation.

**Figure:** MOS transistor test circuit designed in Cadence Virtuoso.

## Output

The simulation data obtained from this circuit is subsequently used to generate the \(g_m/I_D\) lookup curves and determine suitable transistor operating points and dimensions.
