# 🛠️ Freenove Miner

> **Version: v1.8.3.2**

This project utilizes **Freenove ESP32 Display** and **NerdMiner_v2** to implement Bitcoin mining.  
Even if you have no prior knowledge of programming or cryptocurrency, you can easily complete the process by following this tutorial.

🔗 **Project Link:** https://github.com/BitMaker-hub/NerdMiner_v2

---

## 📝 Project Description

**Freenove Miner** is designed for the **Freenove ESP32 Display**, allowing users to experience the process of "mining Bitcoin blocks" through a compact piece of hardware. The main goal of this project is to help more people understand cryptocurrency mining while possessing a beautiful desktop accessory.

<img src="./picture/Freenove Miner(103).png" width="80%">

<img src="./picture/Freenove Miner(112).png" width="80%">

---

## 🖥️ Hardware Support

The following models are fully supported:

- **FNK0103B** (2.8'' ST7789 TN)
- **FNK0103F** (2.8'' ILI9341 TN)
- **FNK0103L** (3.2'' ST7789 IPS)
- **FNK0103N** (3.5'' ST7796 TN)
- **FNK0103S** (4.0'' ST7796 TN)
- **FNK0112** (1.54'' ST7789 IPS)

🛒 **Purchase Links:**

- https://store.freenove.com/products/fnk0103
- https://store.freenove.com/products/fnk0112

🛒 **Amazon**

- https://www.amazon.com/Freenove-NerdMiner-Dual-core-Microcontroller-Tutorial/dp/B0FFZ599FJ
- https://www.amazon.com/FREENOVE-Dual-core-Microcontroller-Programmable-Tutorial/dp/B0G918L5RW

### 📊 Performance Metrics

| Board Model                 | Performance  |
| :-------------------------- | :----------- |
| FNK0103B (2.8'' ST7789 TN)  | **630 KH/s** |
| FNK0103F (2.8'' ILI9341 TN) | **630 KH/s** |
| FNK0103L (3.2'' ST7789 IPS) | **630 KH/s** |
| FNK0103B (2.8'' ST7789 TN)  | **630 KH/s** |
| FNK0103F (2.8'' ILI9341 TN) | **630 KH/s** |
| FNK0112 (1.54'' ST7789 IPS) | **630 KH/s** |

---

## ⛏️ Supported Pools

| Pool URL                | Port  | Web URL                                                   | Status                                                       |
| ----------------------- | ----- | --------------------------------------------------------- | ------------------------------------------------------------ |
| public-pool.io          | 21496 | [https://web.public-pool.io](https://web.public-pool.io/) | Open Source Solo Bitcoin Mining Pool supporting open source miners |
| pool.nerdminers.org     | 3333  | [https://nerdminers.org](https://nerdminers.org/)         | The official Nerdminer pool site - Mantained by @golden-guy  |
| pool.nerdminer.io       | 3333  | [https://nerdminer.io](https://nerdminer.io/)             | Mantained by CHMEX                                           |
| pool.pyblock.xyz        | 3333  | https://pool.pyblock.xyz/                                 | Mantained by curly60e                                        |
| pool.sethforprivacy.com | 3333  | https://pool.sethforprivacy.com/                          | Mantained by @sethforprivacy - public-pool fork              |
| pool.stompi.de          | 3333  | [http://web.stompi.de](http://web.stompi.de/)             | Mantained by @odinstar - public-pool fork                    |
| pool.solomining.de      | 3333  | https://pool.solomining.de/                               | Mantained by https://x.com/solo_mining                       |

Other standard pools not compatible with low difficulty share:

| Pool URL                 | Port | Web URL                                   |
| ------------------------ | ---- | ----------------------------------------- |
| solo.ckpool.org          | 3333 | https://solo.ckpool.org/                  |
| btc.zsolo.bid            | 6057 | https://zsolo.bid/en/btc-solo-mining-pool |
| eu.stratum.slushpool.com | 3333 | https://braiins.com/pool                  |

---

## 📥 Flashing Firmware

### Freenove ESP Web Flasher

<img src="./picture/Freenove web flasher.png" width="70%">

For usage instructions, please refer to the detailed tutorial:
👉 https://docs.freenove.com/projects/fnk0103/en/latest/fnk0103/codes/Miner/NerdMiner_v2.html#how-to-use

---

## ⚙️ Freenove Miner Configuration

After powering on the device, you only need to configure your **Wi-Fi** and **BTC Address**.

📖 **For detailed steps, please refer to:** https://docs.freenove.com/projects/fnk0103/en/latest/fnk0103/codes/Miner/NerdMiner_v2.html#

> ⚠️ **Note**
>
> The BTC address in the default options belongs to Freenove. **You must change it to your own BTC address.**

💡 If you do not own a BTC address yet, please refer to the tutorial: https://docs.freenove.com/projects/fnk0103/en/latest/fnk0103/codes/Miner/Obtaining_the_BTC_Receiving_Address.html#

---

## 🎮 Freenove Miner Usage

### 🌐 Freenove Miner Web Dashboard

On the mining data interface, you can see the device's automatically assigned IP address. Devices connected to the same **Wi-Fi** as the **Freenove Miner** can open the Web Dashboard via this IP address.

> ℹ️ **Tips**:
>
> 1. Data in the Web Dashboard refreshes every **30s**.
>
> 2. Both mobile phones and computers can be used normally.

<img src="./picture/Freenove Miner Dashboard .png" width="80%">

### 🔄 Interface Switching

**Freenove Miner** features four different interfaces:

1. **Mining Data Interface**
2. **Mining Clock Interface**
3. **Global Hashrate Interface**
4. **BTC Price Interface**

#### Button Operations

- **FNK0103**: Short press the `Boot` button on the back to switch.

  > *Note: Since the device devotes most of its computing power to mining, switching may be slightly laggy.*

- **FNK0112**: Tap the **Touch Area** at the top to switch.

#### Touch Screen Operations

- **FNK0103**:
  - Press and hold the **Right half** of the screen: Switch to next interface
  - Press and hold the **Left half** of the screen: Switch to previous interface
- **FNK0112**: Not supported ❌

### ✅ Enable Screen & Serial Debugging

#### WiFi Configuration

In the WiFi configuration interface, you can set this via checkboxes:

*   **Enable Screen**: When checked, the screen is on; when unchecked, the screen is off.
*   **Serial Debugging**: When checked, detailed info is printed to the serial port; when unchecked, only simplified info is printed.

<img src="./picture/Wifi Config.png" width="50%">

#### Web Dashboard Operations

In the Web Dashboard, you can quickly toggle these by clicking the checkboxes, and the miner **will not restart**.

<img src="./picture/Web Config.png" width="50%">

### 🔧 Entering Configuration Mode

#### Button Entry

*   **FNK0103**: Long press the `Boot` button on the back until the Freenove Logo appears on the screen.
*   **FNK0112**: Long press the **Touch Area** until the Freenove Logo appears on the screen.

#### Web Dashboard Settings

Enter the configuration information and click `SAVE & RESTART`.

---

## ❓ FAQ

**Q1: I am a mining beginner, can I easily configure the Freenove Miner?**

> **A:** Absolutely. Configuring the Freenove Miner requires no professional mining knowledge. We provide detailed tutorials to guide you through the process, and our devices come with the Freenove Miner firmware pre-installed.

**Q2: Why is the time displayed correctly after configuration, but mining won't start?**

> **A:** Correct time display indicates a successful WiFi connection, but a failure to connect to the mining pool. Please troubleshoot in this order:
>
> 1. Unplug and replug the USB data cable (network fluctuations might be the cause).
> 2. Check if your router is an ASUS model. If so, you need to turn off the `AiProtection` feature.

**Q3: Why is my miner's max hashrate only around 350? Is my configuration incorrect?**

> **A:** No. If mining starts, your configuration is correct. The reason is likely an outdated firmware version. Please refer to https://docs.freenove.com/projects/fnk0103/en/latest/fnk0103/codes/Miner/NerdMiner_v2.html#how-to-use to download the latest firmware.

**Q4: How do I know if the Freenove Miner is still running after I turn off the screen?**

> **A:** You can verify the current working status via the Freenove Miner Web Dashboard or a Serial Debug Assistant.

**Q5: I see large fluctuations in the hashrate on the pool management interface. Is it unstable?**

> **A:** No. The mining pool estimates hashrate based on the submitted valid shares, so the data will fluctuate. You should refer to the **24H Average Hashrate** or the **Real-time Screen Hashrate**.

**Q6: I have many devices. How do I distinguish them in the pool management interface?**

> **A:** You can add `.WorkerName` after the configured BTC address.
> Example: `bc1qa5...u4l0gu.WorkerName`

---

## 📅 Release Notes

### `v1.8.3.0`(22/12/2025)

*   Deep optimization of the project's screen display for smoother operation.
*   Added support for FNK0112 (1.54'' ST7789 IPS).

### `v1.8.3.1` (09/01/2026)

*   🚀 Boosted hashrate from **340kh/s** to **630kh/s**.
*   Added "Enable Screen & Serial Debugging" function in the miner configuration.

### `v1.8.3.2` (29/01/2026)

*   Added Freenove Miner Web features.
*   Fixed pool data display issues.