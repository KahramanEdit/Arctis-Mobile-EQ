<div align="center">

# 🎮 Arctis Custom EQ

**Unlock the full 10-band Parametric EQ potential of your SteelSeries Arctis headphones!**

[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://android.com)
[![Framework](https://img.shields.io/badge/Framework-LSPosed-blue.svg)](https://github.com/LSPosed/LSPosed)
[![Target](https://img.shields.io/badge/Target-SteelSeries-orange.svg)](https://steelseries.com)
[![License](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)

*Because the mobile app shouldn't limit what your hardware can do.*

</div>

---

## 🚀 Overview

While the PC version of SteelSeries GG allows full parametric EQ adjustments, the official mobile app locks users into pre-made presets. 

**Arctis Custom EQ** is an LSPosed module that bypasses these mobile restrictions. It allows you to create and inject your own custom 10-band Parametric EQ directly into the headset's DSP—**no PC required.**

Whether you want to boost the bass, fine-tune the mids, or adjust the Q-factor (bandwidth) of each frequency, this module gives you full control right from your phone.

## ✨ Features

*   **No PC Required:** Configure deep EQ settings directly from your Android device.
*   **Full 10-Band Control:** Adjust frequencies from 32Hz up to 16kHz.
*   **Gain & Q-Factor:** Control both the volume (Gain) and the width (Q-Factor) of each band.
*   **Modern UI:** A clean, light-themed interface with responsive sliders.
*   **Live Logs:** Built-in log viewer to see exactly when the EQ data is injected.
*   **Seamless Injection:** Hooks directly into the `Nova3BTService` to modify the `Nova3Filter` objects before they are sent to the hardware.

## 📱 Compatibility

*   **Device Tested:** RedMagic 11 Pro (Android 16)
*   **Target App:** SteelSeries Arctis Companion (`com.steelseries.arctiscompanion`)
*   **Headset Tested:** Arctis Nova 3P Wireless 
*(Likely works with Nova 3, Nova 5, and GameBuds as they share the Realtek RTK SDK).*

## 🛠️ Installation

1. Ensure your device is rooted with **Magisk/KernelSU** and **Zygisk** enabled.
2. Install **LSPosed** (Vector version recommended for Android 14+).
3. Download and install the `Arctis-Custom-EQ.apk`.
4. Open LSPosed Manager, enable the module, and set the scope to **SteelSeries Arctis Companion**.
5. Force stop the SteelSeries app and restart it.

## 🎛️ How to Use

1. Open **Arctis Custom EQ**.
2. Toggle **"Modülü Aktif Et"** (Enable Module).
3. Adjust the Gain and Q sliders for your desired frequencies.
4. Open the **SteelSeries Arctis Companion** app.
5. Tap on **any EQ Preset** (e.g., Flat).
6. The module will intercept the command, inject your custom bands, and send them to the headset.

## 🐞 Troubleshooting

* If the sound doesn't change, ensure the module is enabled in LSPosed and the scope is correctly set.
* Use the built-in **LOG** button in the app to verify if `setEQPresetBands -> 10 bant (Filter1-10) guncellendi!` appears in the logs.

---

<div align="center">
  <b>Developed by Clenix / Kahraman</b>
</div>

### ⚠️ Disclaimer & No Liability

*   **Use at your own risk.**
*   This is an unofficial modification. It is not affiliated with, endorsed by, or sponsored by SteelSeries.
*   The developer accepts **NO responsibility** for bricked devices, blown drivers, hearing damage, or any other damage resulting from the use of this software. 
*   Modifying hardware DSP limits may cause audio distortion. Please listen at safe volumes.
