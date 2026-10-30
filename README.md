# URL Checker

🎉 Welcome to **URL Checker 2** (**v16.0.5.1301**, Build 19)!

This release represents a complete modernization, performance overhaul, and fluid frosted-glass UI experience designed for modern Android devices.

## 🌟 What's New & Key Features

* **Live System Background Blurs (Android 12+ / 17):**
  * **Home Screen Wallpaper Diffusion:** `MainActivity` renders directly over the user's live home screen wallpaper using `FLAG_SHOW_WALLPAPER`, transparent window drawables, and deep system background blur (`120.dp` radius), veiled beneath a soft creamy surface tint (`0.84f` alpha).
  * **Contextual App Blur:** When intercepting links from browsers, messaging apps, or social media, `InterceptorActivity` dynamically blurs the active underlying application (`FLAG_BLUR_BEHIND`, radius `110`) beneath a matching creamy frosted scrim.
* **Milky Frosted Glass Materiality:**
  * **Container Blur Decoupling:** `Modifier.blur()` was removed from parent card containers, keeping child text, badges, and icons **100% razor-sharp** with zero cloudy halos or edge distortion.
  * **Uniform Matte Translucency:** Handcrafted frosted translucency across light (`surfaceBright` 84% + `primary` 6%) and dark (`surfaceContainerHigh` 82% + `primaryContainer` 10%) modes, accentuated by subtle `0.03f` anti-banding micro-noise and crisp `1.dp` directional specular borders.
* **Refactored Link Inspection Modal (`InterceptorPopupLayout`):**
  * **Unified Brand Emblem:** Replaced legacy icons with the flat Material 3 `HeroTonalBadge` and Shield-Check emblem (`StickSecurityIcon`), harmonized across the Welcome, About, and Interceptor screens.
  * **Generous URL Headroom:** Expanded destination container to `heightIn(max = 180.dp)` with smooth vertical scrolling and fixed line-height, permanently resolving character slicing on long URLs.
  * **Non-Truncating 2-Tier Actions:** Redesigned bottom actions into a full-width primary pill (`"Open in Browser"`) and a balanced secondary row (`"Cancel"` and `"Scan (VirusTotal)"`), eliminating button label truncation.
* **Polished Screen & Subpage Ergonomics:**
  * **History Screen:** Razor-sharp empty state container with tonal clock badge; `22.dp` rounded cards with zero edge clipping.
  * **Settings Screen & Navigation Pill:** Seamless edge-to-edge layout with `115.dp` bottom scrolling clearance and a floating `CircleShape` frosted navigation capsule with elastic sliding indicators.
  * **Theme & Palette Subpage:** Gliding full-page scroll beneath a pinned frosted header (fixing card clipping); minimalist `40.dp` solid color swatches; single-line title layouts.
  * **Profile Setup Subpage:** Removed nested "box-in-a-box" borders on the Display Name input; standardized all avatar selection circles to an identical `56.dp` with active primary ring indicators.
  * **About & History Management Subpages:** Uniform `22.dp` rounded corners, specular borders, and edge-to-edge system insets.
* **Material 3 Expressive Motion:** Every tap, swipe, and screen transition is powered by physics-based springs (`bounceClickable`, `tiltBounce`, and `ExpressiveSprings`) with tactile overshoot feedback and staggered pop cascades.
* **Modernized Core Toolchain & Tested Stability:** Powered by **Gradle 9.8.2**, **Kotlin 2.4.21**, **Jetpack Compose BOM 2026.09**, **Room 2.8.5**, and **Coroutines 1.11.0**, with a 100% clean test suite across unit, Robolectric, and Roborazzi tests.
* **Ultra-Lightweight APK (~4.4 MB):** Fully optimized with R8 full-mode shrinking and resource stripping (~93% smaller than unoptimized builds).

## 📱 Installation Guide

To install the latest version on your Android device:

1. Go to the **Releases** section on the right side of this repository.
2. Select release **v16.0.5.1301 (Build 19)**.
3. Under the **Assets** section, download `app-release.apk`.
4. Open the downloaded file on your Android device and follow the installation prompts.

## 🛠 Technical Specifications

* **App Version:** `16.0.5.1301` (Version Code `19`)
* **Target SDK:** Android 17 (API 37)
* **Minimum SDK:** Android 12 (API 31)
* **Build System:** Gradle 9.8.2 | AGP 9.4.0
* **Language & UI:** Kotlin 2.4.21 | Jetpack Compose BOM 2026.09.00
* **Data & Networking:** Room 2.8.5 | OkHttp 5.5.0 | Retrofit 3.0.0 | Moshi 1.15.2
* **Optimization:** R8 Full-Mode (`android.enableR8.fullMode=true`), Resource Shrinking, Packaging Exclusions

---
*Maintained at Stable Release v16.0.5.1301 (Build 19)*
