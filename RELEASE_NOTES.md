# 📦 DocDen V1.0.0 Release Notes

**Release Date:** November 4, 2026  
**Build Target:** Android 14 / 15 / 16 (API 34–37)  
**Minimum Supported OS:** Android 7.0 Nougat (API 24)  
**Package Name:** `com.riyuk.docden`  
**Version:** `1.0.0` (VersionCode: `17`)

---

## 🎯 Highlights

- **100% Offline by Design:** No accounts, no cloud servers, no telemetric tracking. Your data remains strictly in your hands.
- **AES-256 Vault Encryption:** Keep confidential IDs, tax records, medical slips, and private notes locked in a military-grade local encrypted vault.
- **Biometric Security:** Secure your vault with Android's native Fingerprint & Face Unlock.
- **Universal Document Viewer:** Built-in fast renderer for PDFs, Microsoft Word (`.docx`), Excel spreadsheets (`.xlsx`), and photos.
- **Seamless Local Backup:** Generate password-protected `.docden` backup bundles to safely transfer data to new devices or external storage.

---

## 📥 Artifact Downloads

| Package Name | Architecture | Recommended For | Description |
| :--- | :--- | :--- | :--- |
| **`DocDen-V1.0.0-universal.apk`** | **Universal (arm64-v8a, armeabi-v7a, x86_64)** | **Android 10+ (Android 10 – 16+)** | **Primary Release.** R8-optimized with uncompressed page-aligned native libraries for instant memory mapping, hardware biometric support, and fluid Material 3 animations. |
| **`DocDen-V1.0.0-android7.apk`** | **Universal (Legacy)** | **Android 7.0 – 9.0** | **Legacy Release.** Compressed libraries tuned for older Android package managers and devices. |

---

## 🔐 Security & Privacy Verification

- **Local Storage:** Everything is stored under `/Android/data/com.riyuk.docden/` and private app sandbox directories.
- **Zero Cloud Calls:** Inspectable with any network monitoring tool—DocDen initiates zero outbound connections.
- **Legal & Policies:** Complete transparency available via in-app Settings and offline Markdown documents:
  - [Privacy Policy](PRIVACY_POLICY.md)
  - [Terms & Conditions](TERMS_AND_CONDITIONS.md)
  - [License](LICENSE)