# Microwave-RF-Communication-Link-Design 📡

This repository contains the design and analysis of a **Point-to-Point (P2P) Microwave Communication Link** operating at **23 GHz**. The project connects two strategic locations in Istanbul—**Kabataş High School (Europe)** and **Üsküdar Nakkaştepe (Asia)**—bridging the Bosphorus with a high-availability wireless link.

The design includes comprehensive path analysis, link budget calculations, and equipment selection to achieve **99.999% availability** (Five Nines) under varying atmospheric conditions.

## 🚀 Project Overview
* **Link Topology:** Point-to-Point (Line-of-Sight).
* **Locations:**
  * **Site A:** Kabataş Erkek Lisesi (41°02'33.0"N, 29°01'18.0"E)
  * **Site B:** Üsküdar Nakkaştepe (41°01'58.0"N, 29°02'21.0"E)
* **Distance:** ~1.85 km.
* **Frequency Band:** 23 GHz (K-Band).
* **Objective:** To design a reliable RF link capable of high-speed data transmission with minimal outage probability.

## Repository Contents

| File | Description |
| :--- | :--- |
| `RF MİKRO PROJE (1).pdf` | Detailed technical report covering site survey, calculations, and equipment datasheet analysis. |
| *(Images/Plots)* | (Optional: Add path profiles or Fresnel zone plots here if available) |

## Design Methodology & Parameters

### 1. Path Analysis & Fresnel Zones
* **Line of Sight (LOS):** Verified using elevation profiles (38m vs 69m AMSL).
* **Fresnel Zone Clearance:** Calculated for the first Fresnel zone (F1) to ensure no obstruction from the Bosphorus strait or urban structures.
  $$R_1 = 17.32 \sqrt{\frac{d_1 d_2}{f \cdot D}}$$

### 2. Link Budget Calculation
The link budget accounts for all gains and losses to determine the **Received Signal Level (RSL)**:
* **Free Space Path Loss (FSPL):** Calculated for 23 GHz over 1.85 km.
  $$FSPL = 92.45 + 20\log(d_{km}) + 20\log(f_{GHz})$$
* **Atmospheric Attenuation:** Losses due to oxygen and water vapor absorption (ITU-R P.676).
* **Rain Attenuation:** Critical for 23 GHz; calculated using ITU-R P.530 for Istanbul's rain zone (Zone K).

### 3. Equipment Selection
* **Radio Unit:** Ericsson MINI-LINK 6363.
* **Antenna:** High-Performance Parabolic Antenna (0.3m / 0.6m diameter).
* **Modulation:** Adaptive modulation (QPSK to 4096-QAM) supported for capacity optimization.

## Key Results

| Parameter | Value |
| :--- | :--- |
| **Operating Frequency** | 23 GHz |
| **Path Distance** | 1.85 km |
| **Antenna Gain** | ~38.5 dBi |
| **Tx Power** | 22 dBm (Max) |
| **Fade Margin** | > 30 dB |
| **Availability Target** | 99.999% (approx. 5 mins outage/year) |

## Site Survey & Map
The link crosses the Bosphorus Strait, requiring precise alignment to mitigate reflection from the water surface and ensuring clearance from maritime traffic.

---
*This project was conducted as part of the Communication Electronics & Microwave Link Design course at Istanbul Technical University.*
