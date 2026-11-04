# Privacy Policy for DocDen

**Effective Date:** November 4, 2026  
**Last Updated:** November 4, 2026  
**Developer:** Riyuk Saha  
**Contact:** [RiyukSaha@gmail.com](mailto:RiyukSaha@gmail.com)

---

At **DocDen**, your privacy and personal data security are our core principles. DocDen is engineered from the ground up as a **100% offline, privacy-first Android application**. We believe your private documents, records, and credentials should belong solely to you, never touching external clouds or surveillance servers.

### 1. 100% Offline Architecture
- DocDen does not connect to any central cloud server, analytics provider, advertisement network, or remote database.
- We do not collect, harvest, store, transmit, or sell any personal data, identifiers, documents, photos, or browsing metadata.
- All documents, databases (Room/SQLite), preferences, and backups exist strictly on your local device storage.

### 2. Local Document Encryption (AES-256)
- Vault documents, notes, tags, person associations, and sensitive files are protected using industry-standard **AES-256** local encryption.
- Encryption keys are stored locally using Android’s secure hardware-backed keystore mechanisms. We do not have backdoor access to your private key or your encrypted documents.

### 3. Biometric Authentication & App Lock
- The App Lock feature utilizes your device's native **Android BiometricPrompt API** (Fingerprint and Face Unlock).
- **DocDen does NOT access, capture, process, or store your biometric samples or templates.**
- Authentication is handled exclusively by your Android operating system and Trusted Execution Environment (TEE) / Secure Element. DocDen only receives a cryptographic success or failure callback from the Android OS.

### 4. Device Permissions Transparency
DocDen requests only the minimal permissions required to provide essential document management features:
- **`USE_BIOMETRIC`**: Enables hardware fingerprint and face authentication for the optional App Lock.
- **Storage / Media Access (`MANAGE_EXTERNAL_STORAGE` / `READ_EXTERNAL_STORAGE`)**: Required exclusively so you can browse, import, view, and back up documents located in your device's file storage. DocDen never scans or indexes files outside your explicit interactions.
- **`POST_NOTIFICATIONS`**: Used solely for local backup completion or local task status indicators.

### 5. Data Retention & Deletion
- Because all data is stored locally on your device, you have complete control over data retention.
- Uninstalling the application or clearing the app’s storage from Android Settings permanently deletes all local data and cryptographic keys from your device.
- You can create and export an encrypted local backup file (`.docden`) at any time via **Settings > Data & Storage > Export Backup**.

### 6. Children's Privacy
DocDen does not collect data from any user, including children under the age of 13.

### 7. Changes to This Privacy Policy
If we update this Privacy Policy to reflect future offline capabilities or legal requirements, the updated version will be packaged with new app releases and committed to this repository with an updated effective date.

### 8. Contact Information
For any questions, concerns, or inquiries regarding this Privacy Policy, please contact:
- **Developer:** Riyuk Saha
- **Email:** [RiyukSaha@gmail.com](mailto:RiyukSaha@gmail.com)
