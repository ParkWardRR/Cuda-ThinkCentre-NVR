# **Cuda-TinyNVR-Build**
 
## **Summary of Specs and Cost**

| **Component**         | **Details**                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| **Base System**       | Lenovo ThinkCentre M920x Tiny (1L form factor, Intel Q370 chipset)          |
| **CPU (Low TDP)**     | Intel Core i5-8600T (6 cores, 6 threads, 2.3GHz base, 3.7GHz boost, 35W TDP)|
| **RAM (32GB DDR4)**   | 2x16GB, 2666MHz                                                             |
| **Storage (NVMe)**    | 512GB NVMe SSD (primary) + 4TB NVMe SSD (video storage)                     |
| **GPU (CUDA Tasks)**  | HP Nvidia Quadro K1200 (512 CUDA cores, 4GB GDDR5)                          |
| **Networking (2.5GbE NIC)** | Intel I225-V Ethernet NIC (M.2 A+E slot, Multi-Gig support)                |
| **Expansion**         | PCIe riser card with GPU faceplate (compatible with T1000 and K1200 GPUs)  |
| **Total Cost**        | **$477 USD (approx.)**                                                      |

---


## **Table of Contents**
1. [Introduction](#introduction)
2. [Specifications](#specifications)
    - [Base System](#base-system)
    - [Processor](#processor)
    - [Networking (2.5GbE NIC)](#networking-25gbe-nic)
    - [Storage](#storage)
    - [Graphics Card (CUDA Tasks)](#graphics-card-cuda-tasks)
    - [Expansion](#expansion)
3. [Cost Breakdown](#cost-breakdown)
4. [Camera and PoE Equipment](#camera-and-poe-equipment)
5. [Networking Setup](#networking-setup)
6. [Software Configuration](#software-configuration)
7. [Notes](#notes)

---

## **Introduction**

This NVR (Network Video Recorder) build is based on a compact **Lenovo ThinkCentre M920x Tiny**, upgraded with a **low-cost, low-wattage Intel Core i5-8600T processor** (35W TDP) for efficient multi-camera video recording, facial recognition, and CUDA-based tasks. The total cost of the build is approximately **$477**, making it an affordable yet powerful solution for NVR applications.

### **Key Features**
- **Compact Design:** 1L ultra-small form factor.
- **Affordable Build:** Uses marketplace prices for cost-effective components.
- **Performance Upgrades:** Enhanced with 32GB RAM, dual NVMe SSDs, and a Quadro K1200 GPU.
- **High-Speed Networking:** Includes 2.5GbE NIC for fast backups to a Synology NAS.
- **Expandable Storage:** Onboard SATA and eSATA options for future upgrades.

> 💡 *All prices are approximate and based on used marketplace values in the USA.*

---

## **Specifications**

### 🖥️ **Base System**
- **Model:** Lenovo ThinkCentre M920x Tiny  
- **Chipset:** Intel Q370  
- **Power Supply:** 135W adapter (88% efficiency)  
- **Storage Options:**
  - Dual M.2 slots for NVMe or Intel Optane memory.
  - Onboard SATA port for additional internal storage.
  - eSATA conversion possible for external drives.

---

### ⚙️ **Processor**
- **Model:** Intel Core i5-8600T (8th Gen Coffee Lake)  
- **Cores/Threads:** 6 cores / 6 threads  
- **Base Frequency:** 2.30 GHz  
- **Max Turbo Frequency:** 3.70 GHz  
- **Cache:** 9MB Intel Smart Cache  
- **TDP:** 35W (energy-efficient design)  
- **Supported Codecs:**
  - Hardware acceleration: H.264, H.265 (HEVC), VP8, VP9.
  - Supports Intel Quick Sync Video for Plex transcoding and media encoding/decoding.

---

### 🌐 **Networking (2.5GbE NIC)**
- **Adapter:** M.2 A+E Intel I225-V Ethernet NIC Card  
    - Multi-Gig support: 2.5GbE / 1GbE / 100Mbps  
    - Use Case: Speeds up video backups to slower storage systems like Synology NAS with spinning drives.

---

### 💾 **Storage**
- **Primary Storage:** TEAMGROUP MP33 512GB NVMe SSD (included with base system).  
- **Additional Storage:** High-capacity 4TB NVMe SSD for video recordings.

---

### 🎮 **Graphics Card (CUDA Tasks)**
- **Installed GPU:** HP Nvidia Quadro K1200  
    - CUDA Cores: 512  
    - Memory: 4GB GDDR5  
    - Use Case: Optimized for CUDA acceleration in facial recognition and AI processing tasks.  
    - Compatibility: T1000 GPU faceplate fits the K1200 perfectly.  
    - Note: Relies on CPU’s Quick Sync Video for Plex transcoding; does not support hardware transcoding itself.

---

### 🔌 **Expansion**
- PCIe expansion riser card:
    - Includes faceplate compatible with Nvidia T1000 and K1200 GPUs.

---

## 💵 **Cost Breakdown**

| Component                              | Price (USD) |
|----------------------------------------|-------------|
| Lenovo ThinkCentre M920x Tiny          | $124.99     |
| Intel Core i5-8600T Processor          | $29.99      |
| Kingston DDR4 RAM (32GB, 2x16GB)       | $32.95      |
| M.2 A+E Intel I225-V Ethernet NIC Card | $28.63      |
| Expansion Riser Card                   | $25.98      |
| 4TB NVMe SSD                           | $200        |
| HP Nvidia Quadro K1200 GPU             | $35         |
| **Total Cost**                         | **$477.54** |

---

## 📷 Camera and PoE Equipment

> ⚠️ *Placeholder*: Add details about cameras, PoE switches, and any other equipment used in the setup.

---

## 🌐 Networking Setup

> ⚠️ *Placeholder*: Add details about IP assignments, VLANs, or how the NVR integrates with your Synology NAS.

---

## 🖥️ Software Configuration

> ⚠️ *Placeholder*: Add details about software used for recording, facial recognition, or system monitoring (e.g., Blue Iris, Frigate).

---

## 📝 Notes

1. The Lenovo ThinkCentre M920x Tiny offers enterprise-grade features:
   - TPM 2.0 security chip.
   - Dual M.2 slots for NVMe or Intel Optane memory.
   - Onboard SATA port allows additional internal storage or eSATA conversion for external drives.

2. The Intel Core i5-8600T processor supports hardware acceleration for H.264, H.265, VP8, and VP9 codecs via Intel Quick Sync Video, making it ideal for Plex transcoding and media-related tasks.

3. The HP Nvidia Quadro K1200 GPU is used exclusively for CUDA-based tasks like facial recognition but is outperformed by newer GPUs like the Nvidia T1000:
   - The T1000 offers nearly double the CUDA cores (896 vs 512) and significantly higher memory bandwidth (~160 GB/s vs ~80 GB/s).
   - However, the K1200 is a cost-effective option at just $35 compared to the T1000’s ~$230 price point while remaining compatible with this build's riser card faceplate.

4. The M.2 A+E Intel I225-V Ethernet NIC provides fast multi-gigabit networking, enabling efficient backups to slower storage systems like a Synology NAS with spinning drives.

5. This build balances cost-effectiveness and performance while leaving room for future storage expansion through onboard SATA or eSATA options.
