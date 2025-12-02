# Privacy Policy - Spender

**Last Updated:** November 22, 2025

## Overview

Spender is built with privacy as a core principle. Your financial data is yours and yours alone. This privacy policy explains how we handle your data (spoiler: we don't).

---

## Our Privacy Commitment

**We collect ZERO data. Period.**

All your financial information, SMS messages, transactions, and personal data remain on your device. We don't have servers, we don't collect analytics, we don't track you, and we never see your data.

---

## Data Collection

### What We Collect
**Nothing.** We do not collect, store, transmit, or access any of your personal or financial data.

### What We DON'T Collect
-  No SMS messages
-  No transaction data
-  No financial information
-  No account numbers or bank details
-  No personal information (name, email, phone, etc.)
-  No location data
-  No usage analytics
-  No crash reports
-  No device identifiers
-  No browsing history
-  No contact information

---

## How Spender Works

### SMS Processing (100% On-Device)
When you enable SMS automation:
- SMS messages are read and processed entirely on your iPhone
- The SMS Analyzer (ML model) runs locally on your device
- No SMS content ever leaves your device
- No SMS data is uploaded to any server (we don't have servers)
- All transaction extraction happens using on-device machine learning

**Technical Implementation:**
- Native ONNX Runtime processes SMS messages locally
- GLiNER model (583MB) runs on your device's processor
- Zero network calls for SMS parsing

### Transaction Data Storage
- All transactions are stored in iOS UserDefaults on your device
- No cloud uploads (unless you enable iCloud Backup - see below)
- No external databases
- No third-party servers

### Machine Learning Model
The SMS Analyzer is a 583MB machine learning model that you optionally download:
- **Download Source:** Apple's Content Delivery Network (CDN) via On-Demand Resources
- **Download Process:** Standard iOS system download, same as downloading app updates
- **Model Storage:** Stored locally on your device
- **Model Usage:** Runs entirely on your device, no network calls during inference
- **Privacy:** Model never sends data anywhere

---

## Optional Features & Privacy

### iCloud Backup (Optional)
If you enable iCloud Backup in Settings:
- Backup data is encrypted and stored in **your personal iCloud account**
- We never have access to your iCloud data
- Apple's standard iCloud privacy policies apply
- You can disable iCloud Backup anytime
- Backups include: transactions, accounts, categories, settings

**Important:** iCloud Backup uses YOUR iCloud storage, not our servers (we don't have servers).

### Local XML Backup (Optional)
You can create encrypted local backups:
- Backups are saved to your device's Files app
- You control where to store the backup file
- Encrypted with iOS standard encryption
- You can share/store backups wherever you want (Dropbox, Google Drive, email, etc.)

### Currency Exchange Rates
For currency conversion, we fetch exchange rates from:
- **Source:** Public GitHub CDN (fawazahmed0/currency-api)
- **Data Transmitted:** Currency code requests (e.g., "USD to EUR rate")
- **No Personal Data:** These requests contain no personal or financial information
- **Offline Fallback:** Bundled rates work without internet

---

## Third-Party Services & SDKs

### ONNX Runtime (Objective-C)
The only third-party component in Spender is ONNX Runtime for running the ML model:
- **Purpose:** On-device machine learning inference
- **Privacy:** Runs entirely offline, no network calls
- **License:** MIT License
- **Data Access:** Only processes data you provide locally

### No Analytics or Tracking SDKs
We do NOT use:
-  Google Analytics
-  Firebase Analytics
-  Facebook SDK
-  Crashlytics
-  Mixpanel
-  Segment
-  Any other analytics or tracking tools

### No Advertising
-  No ad networks
-  No ad tracking
-  No personalized advertising
-  No data sold to advertisers

---

## Permissions

### SMS Permission (Optional)
- **Purpose:** Read bank transaction SMS messages for automatic parsing
- **Scope:** Only when you enable SMS automation and download SMS Analyzer
- **Processing:** 100% on-device, never uploaded
- **Control:** You can revoke this permission anytime in iOS Settings

### iCloud Permission (Optional)
- **Purpose:** Backup to your personal iCloud account
- **Scope:** Only if you enable iCloud Backup in Settings
- **Access:** We never access your iCloud data
- **Control:** You can disable iCloud Backup anytime

### No Other Permissions
We do NOT request:
-  Location access
-  Camera access (except for CSV file import via document picker)
-  Contacts access
-  Microphone access
-  Photo library access (except for document import)
-  Calendar access
-  Bluetooth access

---

## Data Retention

### On Your Device
- All data is stored on your device indefinitely
- You control data retention
- Delete transactions anytime - they're immediately removed
- Uninstall the app to delete all local data

### In iCloud (If Enabled)
- iCloud backups follow Apple's iCloud retention policies
- Delete backups anytime from Settings † Backup & Restore
- Disable iCloud Backup to stop future uploads

### On Our Servers
**We don't have servers.** There's nothing to retain.

---

## Your Rights & Control

You have complete control over your data:

###  Full Data Ownership
- All data belongs to you
- No license to us
- No terms of service claiming data rights

###  Export Data Anytime
- Export to CSV format (Excel, Google Sheets compatible)
- Export to QIF format (finance app compatible)
- Export to OFX format (accounting software compatible)
- Export to XML format (complete backup)

###  Delete Data Anytime
- Delete individual transactions
- Delete entire accounts
- Clear all data from Settings
- Uninstall app to remove everything

###  No Account Required
- No sign-up
- No login
- No email verification
- No phone number verification
- Complete anonymity

---

## Children's Privacy

Spender does not collect data from anyone, including children under 13. Since we don't collect any data, we comply with COPPA (Children's Online Privacy Protection Act) by default.

---

## Changes to Privacy Policy

We may update this privacy policy occasionally. Changes will be communicated through:
- App updates with release notes
- Updated "Last Updated" date at the top of this document
- Notification in the app (for major changes)

Continued use of Spender after changes means you accept the updated policy.

---

## International Privacy

Spender respects international privacy laws:

### GDPR (Europe)
- **Lawful Basis:** Not applicable - we don't collect data
- **Data Controller:** Not applicable - no data processing
- **Data Subject Rights:** You control all data (it's on your device)
- **Data Portability:** Export to CSV/QIF/OFX anytime
- **Right to Erasure:** Delete data anytime

### CCPA (California)
- **Data Sale:** We don't sell data (we don't have data to sell)
- **Data Collection:** None
- **Opt-Out Rights:** Not applicable - nothing to opt out of

---

## Security

While we don't collect your data, we take security seriously:

### On-Device Security
- All data encrypted by iOS sandbox
- iOS UserDefaults with standard encryption
- No network transmission of sensitive data
- Local ML processing only

### iCloud Security (If Enabled)
- Apple's standard iCloud encryption applies
- End-to-end encryption for backup data
- Two-factor authentication recommended (your Apple ID)

### No Server Security Needed
- We don't have servers
- No server breaches possible
- No centralized database to hack

---

## Contact Us

If you have questions about this privacy policy or Spender's privacy practices:

- **Email:** spender-support@gmail.com
- **Subject Line:** "Privacy Policy Question"
- **Response Time:** Within 24-48 hours

For bug reports or feature requests, see our [Support Guide](SUPPORT.md).

---

## Legal

This privacy policy is effective as of the "Last Updated" date above.

Spender is developed by an independent developer and is not affiliated with any financial institution, bank, or payment processor.

**Disclaimer:** While we prioritize privacy and security, you are responsible for:
- Securing your iOS device (passcode, Face ID, Touch ID)
- Managing your iCloud account security
- Keeping backup files secure if exported
- Understanding that SMS messages on your device may be accessible to other apps with SMS permissions

---

## Summary (TL;DR)

 **Zero data collection** - We don't collect anything
 **100% on-device processing** - SMS parsing happens locally
 **No servers** - All data stays on your iPhone
 **No analytics** - We don't track you
 **Optional iCloud** - Uses YOUR iCloud, we can't access it
 **Full control** - Export, delete, or keep your data forever
 **No ads** - Never

Your financial privacy matters. That's why Spender was built this way.

---

*For the full feature list, installation guide, and FAQ, see our [README](README.md).*

*For technical support, see our [Support Guide](SUPPORT.md).*

---

**Copyright Â© 2025. All rights reserved.**
