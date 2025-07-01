# 📱 Unit Converter App

A simple and clean Android app to convert between metric and imperial units, built using **Kotlin** and **Jetpack Compose**.

---

## ✨ Features

- 🔁 Unit conversion in real-time
- 🎯 Accurate results (rounded to 2 decimal places)
- 📐 Supported units:
  - Meters
  - Centimeters
  - Millimeters
  - Feet
- 📱 Modern UI using **Material 3**
- ⚡ Lightweight, fast, and responsive

---

## 📦 Download

Grab the latest APK from the [Releases](https://github.com/Pradip1010100/UnitConverter/releases) section.

---

## 🧮 Conversion Logic

All units are internally converted to meters using a conversion factor:

```kotlin
val result = (inputValue * iConversionFactor * 100.0 / oConversionFactor).roundToInt() / 100.0
