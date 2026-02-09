# Microwave-RF-Communication-Link-Design 📡

This repository contains the design and analysis of a **Point-to-Point (P2P) Microwave Communication Link** operating in the **8 GHz** band. The project connects two strategic locations in Istanbul—**Kabataş High School (Europe)** and **Üsküdar Nakkaştepe (Asia)**—bridging the Bosphorus with a high-availability wireless link.

The design utilizes **Space Diversity** to mitigate multipath fading and aims for an ultra-high availability target of **99.9999%** (approx. 5 seconds outage per year).

## Project Overview
* **Link Topology:** Point-to-Point (Line-of-Sight).
* **Locations:**
  * **Site A:** Kabataş Erkek Lisesi (Europe)
  * **Site B:** Üsküdar Nakkaştepe (Asia)
* **Frequency Band:** **8 GHz** (ITU-R F.386-9 Standard).
* **Diversity Technique:** **Space Diversity** (Selected over Frequency Diversity for better gain and fade margin).
* **Objective:** To design a carrier-grade RF link capable of uninterrupted data transmission across the Bosphorus Strait.

## Repository Contents

| File | Description |
| :--- | :--- |
| `RF MİKRO PROJE (1).pdf` | Detailed technical report covering site survey, calculations, and equipment datasheet analysis. |
| *(Images/Plots)* | (Optional: Add path profiles or Fresnel zone plots here if available) |

## Design Methodology & Parameters

### 1. Frequency & Channel Planning
* **Operating Band:** **7.1 GHz - 8 GHz** range.
* **Standard:** Compliance with **ITU-R F.386-9** channel arrangements.
* **Selection Logic:** The 8 GHz band was chosen to balance path loss and rain attenuation suitable for the link distance and regional climate.

### 2. Path Analysis
* **Line of Sight (LOS):** Confirmed path clearance over the Bosphorus strait.
* **Fresnel Zones:** Analysis ensures the first Fresnel zone is free from obstructions (sea surface reflections and maritime traffic).

### 3. Diversity & Availability
* **Space Diversity:** Implemented to counteract multipath fading, which is critical for water-crossing links.
* **Target Availability:** **99.9999%** (Six Nines).
* **Outage Tolerance:** Calculated to be approximately **5 seconds per year**.

## Key Results

| Parameter | Value |
| :--- | :--- |
| **Operating Frequency** | **8 GHz** |
| **Antenna Configuration** | Space Diversity (Main + Diversity Antennas) |
| **Availability Target** | **99.9999%** |
| **Fade Margin** | Optimized for >40 dB (with Diversity) |
| **Rain Zone** | ITU-R Zone K (Istanbul) |

## Site Survey
The link crosses the Bosphorus Strait, requiring precise antenna alignment and height planning to mitigate **surface reflections** (tidal effects) and ensure clearance for large vessels passing through the strait.

---
*This project was conducted as part of the **EHB 473 Microwave and RF Communication** course at Istanbul Technical University.*
