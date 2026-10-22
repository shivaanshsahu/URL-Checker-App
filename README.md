# URL Checker

🎉 Welcome to **URL Checker 2** (**v16.0.5.1201**, Build 18)!

This release represents a complete modernization, performance overhaul, and fluid UI experience designed for modern Android devices.

## 🌟 What's New & Key Features

* **Material 3 Expressive Motion:** Every tap, swipe, and screen transition is now driven by fluid spring physics (`bounceClickable`, `tiltBounce`, and `ExpressiveSprings`). Features tactile overshoot feedback, card pop-in entries, staggered list cascades, and elastic navigation pill sliding.
* **Target Android 17 (API 37):** Upgraded to target the latest Android 17 platform while maintaining seamless compatibility and performance for Android 12+ (API 31+).
* **Massive APK Size Reduction (~93% Smaller):** Configured with R8 full-mode shrinking, resource stripping, and release log removal, shrinking the final package from 66 MB down to just **4.4 MB**.
* **Modernized Core Toolchain & Libraries:** Powered by the latest stable **Gradle 9.8.2**, **Kotlin 2.4.21**, **Jetpack Compose BOM 2026.09**, **Room 2.8.5**, and **Coroutines 1.11.0**.
* **Deep Architectural & Logic Fixes:** Resolved redirect loop edge cases with hop guards, optimized Room database concurrency, corrected IME insets for modern edge-to-edge displays, and eliminated background leak vectors.
* **Verified Test Suite:** All Robolectric, unit, and screenshot test suites run cleanly with a 100% pass rate.

## 📱 Installation Guide

To install the latest version on your Android device:

1. Go to the **Releases** section on the right side of this repository.
2. Select release **v16.0.5.1201 (Build 18)**.
3. Under the **Assets** section, download `app-release.apk`.
4. Open the downloaded file on your Android device and follow the installation prompts.

## 🛠 Technical Specifications

* **App Version:** `16.0.5.1201` (Version Code `18`)
* **Target SDK:** Android 17 (API 37)
* **Minimum SDK:** Android 12 (API 31)
* **Build System:** Gradle 9.8.2 | AGP 9.4.0
* **Language & UI:** Kotlin 2.4.21 | Jetpack Compose BOM 2026.09.00
* **Data & Networking:** Room 2.8.5 | OkHttp 5.5.0 | Retrofit 3.0.0 | Moshi 1.15.2
* **Optimization:** R8 Full-Mode (`android.enableR8.fullMode=true`), Resource Shrinking, Packaging Exclusions

---
*Maintained at Stable Release v16.0.5.1201 (Build 18)*
