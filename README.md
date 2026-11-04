<div align="center">

<img src="DocDen.svg" alt="DocDen Logo" width="130" height="130" style="border-radius: 24px;" />

# DocDen

**The Secure, Encrypted, 100% Offline Document Vault & Manager for Android.**  
*Built with modern Kotlin, Jetpack Compose, and Material 3 Expressive design.*

<p align="center">
  <a href="#">
    <img src="https://img.shields.io/badge/Version-v1.0.0-10B981?style=for-the-badge&labelColor=0d1f18" alt="Version v1.0.0" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Security-AES--256%20GCM-00E5FF?style=for-the-badge&labelColor=02262b" alt="AES-256 Encryption" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Privacy-100%25%20Offline-7C3AED?style=for-the-badge&labelColor=1a0c2e" alt="100% Offline" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Platform-Android%207.0%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white&labelColor=132b1d" alt="Android 7.0+" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/License-Proprietary-EF4444?style=for-the-badge&labelColor=2b0e0e" alt="Proprietary License" />
  </a>
</p>

<p align="center">
  <a href="#-key-features">Features</a> •
  <a href="#-download-packages">Downloads</a> •
  <a href="#-security--privacy-architecture">Security</a> •
  <a href="#-legal--policies">Legal & Policies</a>
</p>

</div>

---

## 🌟 Overview

**DocDen** is an ultra-secure, privacy-first personal document vault engineered for users who value absolute sovereignty over their data. Unlike conventional cloud document services that expose your private IDs, medical files, tax receipts, and contracts to remote data breaches, **DocDen operates strictly 100% offline**.

All documents, tags, person associations, and metadata are encrypted directly on your device hardware using **AES-256 GCM**. Protected by an effortless **Biometric App Lock** (Fingerprint & Face Unlock) and wrapped in a stunning **Material 3 Expressive** interface, DocDen makes private document management smooth, reliable, and aesthetically delightful.

---

## ✨ Key Features

### 🛡️ Local AES-256 GCM Encrypted Vault
- **Zero-Knowledge Architecture:** Encrypt sensitive documents, IDs, passport copies, financial records, and private notes directly inside your device's isolated storage sandbox.
- **Hardware-Backed Key Derivation:** Cryptographic keys are bound to your device using Android's hardware security layer.

### 🔒 Native Hardware Biometric App Lock
- **Fingerprint & Face Unlock:** Direct integration with Android's native `BiometricPrompt` framework.
- **Privacy Preserving:** Zero biometric data is ever viewed or stored by DocDen; all checks occur within the Android operating system Trusted Execution Environment (TEE).
- **Instant Background Timeout:** Automatically locks the vault the moment you switch apps or lock your screen.

### 📄 Universal Document & File Viewer
- **Multi-Format Rendering:** Built-in high-performance viewer for **PDFs**, Microsoft Word (**`.docx`**), Microsoft Excel (**`.xlsx`**), text files, and high-resolution images.
- **Theme Adaptability:** Automatic day and night mode switching for document reading without eye strain.

### 👥 People & Smart Tag Organization
- **People Tagging:** Attach documents to family members, clients, or doctors with profile photos, date of birth, age calculation, and contact notes.
- **Color-Coded Tags:** Organize files with customizable tag color palettes and nested folders for effortless document discovery.
- **Instant Offline Search:** Filter and search across thousands of files, file extensions, people, and tags in milliseconds.

### 💾 Encrypted Portable Backups (`.docden`)
- **One-Click Backup & Restore:** Export your entire vault, documents, relationships, and metadata into a single AES-256 encrypted `.docden` archive file.
- **Offline Data Migration:** Easily restore your complete vault to a new device without relying on internet connectivity.

### 🎨 Material 3 Expressive Theming
- **Dynamic Accent Colors:** Choose from preset palettes or pick your own custom accent hue.
- **AMOLED True-Black Mode:** Completely deep pitch-black backgrounds tailored for battery efficiency on OLED displays.
- **Fluid Gestures:** Expressive bottom sheets, spring animations, and edge-to-edge system bar integration.

---

## 📦 Download Packages

We provide pre-compiled, optimized APKs built via our automated CI/CD workflow. Check the [Releases](../../releases) tab to download.

| Package | Recommended OS | Architecture | Highlights |
| :--- | :--- | :--- | :--- |
| **`DocDen-V1.0.0-universal.apk`** | **Android 10+ (API 29–37)** | Universal (`arm64-v8a`, `armeabi-v7a`, `x86_64`) | **Standard Recommended Release.** R8-optimized with page-aligned uncompressed native libraries. |
| **`DocDen-V1.0.0-android7.apk`** | **Android 7.0 – 9.0 (API 24–28)** | Universal (Legacy) | **Legacy Variant.** Built with compressed native libraries for older package managers. |

---

## 🔐 Security & Privacy Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                       DocDen App                            │
├──────────────────────────────┬──────────────────────────────┤
│    Presentation (Compose M3) │  BiometricPrompt Gate        │
├──────────────────────────────┴──────────────────────────────┤
│              Domain & Local Repository Layer                │
├──────────────────────────────┬──────────────────────────────┤
│    Room DB (Encrypted Meta)  │  AES-256 GCM Cipher Stream   │
├──────────────────────────────┴──────────────────────────────┤
│           Android Hardware Sandbox & Keystore (TEE)         │
│           - Zero Network Outbound Sockets                   │
│           - 100% Offline Device Storage                     │
└─────────────────────────────────────────────────────────────┘
```

1. **Zero Outbound Connections:** DocDen does not ping remote APIs, telemetry backends, or crash analytics.
2. **Encrypted at Rest:** Files stored in the vault are chunked and encrypted with unique initialization vectors (IV).
3. **No Account Required:** Start using the app immediately with zero sign-ups or email registrations.

---

## 📜 Legal & Policies

DocDen values full transparency, copyright protection, and respects the open-source community:

- 🔒 **[Privacy Policy](PRIVACY_POLICY.md)** — Our strict zero-data collection guarantee and biometric privacy disclosures.
- ⚖️ **[Terms and Conditions](TERMS_AND_CONDITIONS.md)** — Software usage agreement, user data responsibility, and liability limitations.
- 📄 **[License](LICENSE)** — Proprietary & Confidential Software License (Copyright © 2024–2026 Riyuk Saha. All Rights Reserved).
- 📝 **[Changelog](CHANGELOG.md)** — Chronological release history and new features.
- 🤝 **Credits:** DocDen integrates visual architectures and UI frameworks adapted from the open-source LastWave-Native project. We deeply acknowledge the foundational work by Clash-Projects. Original Repository: [LastWave-native](https://github.com/Clash-Projects/LastWave-native).

---

## 👤 Developer & Maintainer

- **Developer:** Riyuk Saha
- **Contact:** [RiyukSaha@gmail.com](mailto:RiyukSaha@gmail.com)
- **Application ID:** `com.riyuk.docden`

<div align="center">
  <sub>Copyright © 2024–2026 Riyuk Saha. All Rights Reserved.</sub>
</div>