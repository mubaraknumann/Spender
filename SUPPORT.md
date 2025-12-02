# Spender Beta - Support Guide

**Need help? You're in the right place.**

This guide covers common issues, setup instructions, troubleshooting, and how to get help.

---

##  Contact Support

### Email Support
- **Email:** numanmubarak@protonmail.com
- **Response Time:** Within 24-48 hours
- **Support Hours:** 9 AM - 9 PM IST (Monday-Saturday)

### What to Include in Support Emails
To help us assist you faster, please include:
- **iOS Version:** (e.g., iOS 17.1)
- **Device Model:** (e.g., iPhone 14 Pro)
- **App Version:** (Settings † About † Version)
- **Issue Description:** What happened vs. what you expected
- **Steps to Reproduce:** How can we recreate the issue?
- **Screenshots:** If applicable (hide sensitive financial data)

---

##  Getting Started

### First-Time Setup (5 Minutes)

1. **Install the App**
   - Download from App Store (see [README](README.md#installation))
   - Open Spender Beta on your iPhone

2. **Explore the Dashboard**
   - The dashboard shows your financial overview
   - Initially empty - let's add some data

3. **Add Your First Transaction (Manual)**
   - Tap the **+** button
   - Fill in: Amount, Description, Account, Category, Date
   - Tap **Save**
   - See it appear in your transaction list

4. **Set Up Accounts**
   - Go to **Settings † Accounts**
   - Tap existing accounts to set starting balances
   - Or add new accounts manually

5. **Optional: Enable SMS Automation**
   - Only if you want automatic SMS capture
   - See [SMS Automation Setup](#sms-automation-setup) below

---

##  SMS Automation Setup

### Requirements
-  iOS 26.0 or later
-  600MB+ free storage space
-  WiFi connection (for downloading SMS Analyzer)
-  Bank transaction SMS messages

### Step-by-Step Setup

#### Step 1: Download SMS Analyzer
1. Open Spender Beta
2. Go to **Settings † SMS Analyzer**
3. Tap **"Download SMS Analyzer"**
4. **Keep the app open** while downloading (2-5 minutes)
5. Wait for "Download Complete" message

**Troubleshooting:**
- If download fails, check free storage space (need 600MB+)
- Ensure WiFi is connected (don't use cellular for large downloads)
- Try closing and reopening the app, then retry download
- If stuck, force quit app and try again

#### Step 2: Create iOS Shortcut
1. In Settings † Automation, tap **"Setup Shortcut"**
2. Follow iOS prompts to create automation
3. Grant SMS permissions when asked
4. Test with a bank SMS message

#### Step 3: Enable SMS Automation
1. In Settings † Automation, toggle **"SMS Automation"** ON
2. You're done! New bank SMS messages will be processed automatically

### What SMS Messages Work?
The SMS Analyzer recognizes transaction SMS from:
-  All major banks
-  Credit card companies
-  Digital wallets
-  UPI payment notifications

**Format Requirements:**
- Must contain transaction amount
- Must indicate debit/credit/payment
- Must have identifiable account or card info
- Works best with standard bank SMS formats

---

##  Troubleshooting

### SMS Messages Not Being Processed

**Symptom:** SMS messages arrive but no transactions appear in app

**Possible Causes & Solutions:**

1. **SMS Analyzer Not Downloaded**
   - **Check:** Settings † SMS Analyzer † Status should say "Downloaded"
   - **Fix:** Download the SMS Analyzer (see [SMS Automation Setup](#sms-automation-setup))
   - **Important:** SMS automation REQUIRES the SMS Analyzer - it won't work without it

2. **SMS Automation Disabled**
   - **Check:** Settings † Automation † "SMS Automation" should be ON
   - **Fix:** Toggle SMS Automation ON

3. **iOS Shortcut Not Set Up**
   - **Check:** iOS Shortcuts app should have a Spender automation
   - **Fix:** Settings † Automation † "Setup Shortcut" † Follow prompts

4. **SMS Permissions Not Granted**
   - **Check:** iOS Settings † Spender † Should have SMS access
   - **Fix:** Grant SMS permissions in iOS Settings

5. **Non-Transaction SMS**
   - **Check:** Is the SMS actually a bank transaction message?
   - **Fix:** SMS Analyzer only processes transaction SMS (debits, credits, payments)

6. **Unsupported SMS Format**
   - **Check:** Is it from a recognized bank/financial service?
   - **Fix:** Try manual entry for non-standard formats, or report the SMS format to us

### Incorrect Account Balances

**Symptom:** Account balance doesn't match your expectations

**Possible Causes & Solutions:**

1. **Starting Balance Not Set**
   - **Check:** Settings † Accounts † Tap account † Starting Balance
   - **Fix:** Set the correct starting balance for each account

2. **Duplicate Transactions**
   - **Check:** Look for duplicate entries in transaction list
   - **Fix:** Delete duplicate transactions (swipe left † Delete)

3. **Missing Transactions**
   - **Check:** Filter transactions by account to see all entries
   - **Fix:** Add missing transactions manually

4. **Merged Accounts Not Reflected**
   - **Check:** Settings † Accounts † Verify merged accounts show correct target
   - **Fix:** Re-merge accounts if needed

5. **Transfer Counted Twice**
   - **Check:** Look for both debit and credit for same transfer
   - **Fix:** Delete one side of the transfer, or mark one as "Personal Transfer"

### SMS Analyzer Download Fails

**Symptom:** Download starts but doesn't complete or shows error

**Possible Causes & Solutions:**

1. **Insufficient Storage Space**
   - **Check:** iOS Settings † General † iPhone Storage
   - **Fix:** Free up at least 600MB of space (delete apps, photos, or files)

2. **Poor Internet Connection**
   - **Check:** WiFi signal strength
   - **Fix:** Move closer to router, or try different WiFi network

3. **Using Cellular Data**
   - **Check:** Is WiFi actually connected?
   - **Fix:** iOS may block large downloads on cellular - use WiFi

4. **App Backgrounded During Download**
   - **Check:** Did you close the app during download?
   - **Fix:** Keep app open and phone unlocked during download

5. **Apple CDN Issues**
   - **Check:** Try again in 5-10 minutes
   - **Fix:** Temporary server issues usually resolve quickly

### iCloud Backup Not Working

**Symptom:** iCloud Backup enabled but not syncing

**Possible Causes & Solutions:**

1. **iCloud Not Logged In**
   - **Check:** iOS Settings † [Your Name] † iCloud
   - **Fix:** Sign in to iCloud

2. **iCloud Storage Full**
   - **Check:** iOS Settings † [Your Name] † iCloud † Manage Storage
   - **Fix:** Free up iCloud space or upgrade storage plan

3. **iCloud Drive Disabled**
   - **Check:** iOS Settings † [Your Name] † iCloud † iCloud Drive
   - **Fix:** Enable iCloud Drive

4. **Network Issues**
   - **Check:** WiFi connection
   - **Fix:** Ensure stable internet connection for backup

### CSV Import Issues

**Symptom:** CSV file won't import or imports incorrectly

**Possible Causes & Solutions:**

1. **Wrong CSV Format**
   - **Check:** CSV should have headers (Date, Amount, Description, etc.)
   - **Fix:** See [CSV Import Guide](#csv-import-guide) below for format

2. **Date Format Not Recognized**
   - **Check:** Dates should be in recognizable format (YYYY-MM-DD, DD/MM/YYYY, etc.)
   - **Fix:** Reformat dates in Excel/Google Sheets before export

3. **Amount Format Issues**
   - **Check:** Amounts should be numbers (1234.56), not formatted with currency symbols
   - **Fix:** Remove currency symbols and commas from CSV

4. **Duplicate Transactions**
   - **Check:** Spender skips duplicates - is it intentional?
   - **Fix:** This is normal behavior to prevent duplicate imports

### App Crashes or Freezes

**Symptom:** App becomes unresponsive or closes unexpectedly

**Possible Causes & Solutions:**

1. **Low Memory**
   - **Check:** Close other apps running in background
   - **Fix:** Restart your iPhone

2. **Corrupted Data**
   - **Check:** Does crash happen when viewing specific transaction or account?
   - **Fix:** Try deleting that transaction or create backup and reinstall app

3. **iOS Bug**
   - **Check:** Is iOS up to date?
   - **Fix:** Update to latest iOS version (Settings † General † Software Update)

4. **App Bug**
   - **Check:** Is Spender Beta up to date?
   - **Fix:** Update from App Store, or report crash to support

**Always report crashes via email with:**
- What you were doing when it crashed
- Steps to reproduce
- Device and iOS version

---

##  CSV Import Guide

### Supported Formats
- **CSV** (Comma-Separated Values) - Excel, Google Sheets
- **QIF** (Quicken Interchange Format) - Other finance apps
- **OFX** (Open Financial Exchange) - Accounting software

### CSV File Structure

**Minimum Required Columns:**
- Date
- Amount
- Description (or Merchant)

**Optional Columns:**
- Account
- Category
- Type (Income, Expense, Transfer, Payment)
- Notes

**Example CSV:**
```csv
Date,Amount,Description,Account,Category,Type
2024-01-15,50.00,Grocery Store,HDFC Savings,Food & Dining,Expense
2024-01-16,5000.00,Salary,HDFC Savings,Income,Income
2024-01-17,1200.00,Rent Payment,HDFC Savings,Rent,Expense
```

### Import Steps
1. Go to **Settings † Import/Export † Import Transactions**
2. Select **CSV File**
3. Choose file from Files app
4. Review column mapping (auto-detected)
5. Adjust mappings if needed
6. Tap **Import**
7. Review summary (imported vs. duplicates skipped)

---

##  Data Export Guide

### Export Formats
- **CSV** - For Excel, Google Sheets, Numbers
- **QIF** - For other finance apps (Quicken, YNAB, etc.)
- **OFX** - For accounting software (QuickBooks, etc.)
- **XML** - Complete backup with all settings

### Export Steps
1. Go to **Settings † Import/Export † Export Transactions**
2. Select format (CSV, QIF, OFX, or XML)
3. Choose date range or "All Transactions"
4. Tap **Export**
5. Save to Files app or share via email/cloud

### When to Export
-  Regular backups (weekly/monthly)
-  Before app reinstall or iOS upgrade
-  To analyze data in Excel/Google Sheets
-  To migrate to another finance app
-  For tax records or accounting

---

##  Account Management

### Adding Accounts
1. **Automatic Discovery:** Accounts are auto-discovered from transactions
2. **Manual Addition:** Settings † Accounts † Add Account

### Setting Starting Balances
1. Go to **Settings † Accounts**
2. Tap the account
3. Tap **"Set Starting Balance"**
4. Enter balance as of first transaction date
5. Tap **Save**

**Important:** Starting balance should be the account balance BEFORE your first tracked transaction.

### Merging Duplicate Accounts
If you have duplicate accounts (e.g., "HSBC Bank" and "HSBC"):

1. Go to **Settings † Accounts**
2. Tap the **duplicate account** (source)
3. Tap **"Merge Account"**
4. Select **target account** to merge into
5. Tap **Confirm**

**Result:** All transactions from source account are moved to target account. Starting balance is preserved.

### Account Types
- **Savings** - Bank savings account (asset)
- **Checking** - Bank checking account (asset)
- **Credit Card** - Credit card (liability)
- **Wallet** - Digital wallet or cash (asset)

---

##  Categories

### Default Categories
Spender Beta includes 13 default categories:
- Food & Dining
- Shopping
- Transport
- Bills & Utilities
- Entertainment
- Healthcare
- Travel
- Education
- Income
- Rent
- Investment
- Personal Transfer
- Uncategorized

### Creating Custom Categories
1. Go to **Settings † Categories**
2. Tap **"Add Category"**
3. Enter category name
4. Choose color and icon (if available)
5. Tap **Save**

### Changing Transaction Categories
1. Tap a transaction
2. Tap **Category** field
3. Select new category
4. Tap **Save**

**Tip:** Check "Apply to all transactions from this merchant" to auto-categorize future transactions.

---

##  Backup & Restore

### Local XML Backup (Recommended)

**Create Backup:**
1. Go to **Settings † Backup & Restore**
2. Tap **"Create Backup"**
3. Save XML file to Files app
4. **Store securely** (iCloud Drive, Google Drive, email to yourself, etc.)

**Restore Backup:**
1. Go to **Settings † Backup & Restore**
2. Tap **"Restore from Backup"**
3. Select XML file
4. Confirm restoration
5. App will reload with restored data

**Backup Contents:**
- All transactions
- All accounts (with starting balances)
- All categories (default + custom)
- Account merge history
- App settings

### iCloud Backup (Optional)

**Enable iCloud Backup:**
1. Go to **Settings † Backup & Restore**
2. Toggle **"iCloud Backup"** ON
3. Initial backup starts automatically
4. Future backups are automatic

**Restore from iCloud:**
1. Install app on new device
2. Sign in with same Apple ID
3. Go to Settings † Backup & Restore
4. Tap **"Restore from iCloud"**
5. Select backup to restore

**Important:** iCloud backup requires:
- Signed in to iCloud (iOS Settings † [Your Name])
- iCloud Drive enabled
- Sufficient iCloud storage space

---

##  Privacy & Security

### Your Data is Private
- All processing happens on your device
- SMS Analyzer runs locally (no server calls)
- No data uploaded to external servers
- No analytics or tracking

### Securing Your Data
**Best Practices:**
- Enable iPhone passcode/Face ID/Touch ID
- Don't share iPhone with others
- Create regular backups
- Store backup files securely
- Don't share screenshots with account numbers visible

### iCloud Privacy
- iCloud backups use YOUR personal iCloud account
- We never access your iCloud data
- Apple's iCloud encryption applies
- Enable two-factor authentication on Apple ID

For full privacy details, see our [Privacy Policy](PRIVACY_POLICY.md).

---

##  FAQ

For comprehensive FAQ covering setup, usage, and troubleshooting, see:
- **In-App FAQ:** Settings † FAQ & Help
- **Online FAQ:** [README - FAQ Section](README.md#faq)

### Quick FAQ

**Q: Do I need to download the SMS Analyzer?**
A: Only if you want SMS automation. The app works perfectly with manual entry and file imports without it.

**Q: How much storage does the SMS Analyzer require?**
A: 583MB. Ensure you have 600MB+ free space before downloading.

**Q: Is my data safe?**
A: Absolutely. All processing happens on your device. Your SMS and transaction data never leave your iPhone.

**Q: Can I use Spender on multiple devices?**
A: Yes, via iCloud Backup. Enable iCloud Backup on both devices (same Apple ID) for automatic sync.

**Q: How do I backup my data?**
A: Two ways - Local XML Backup (Settings † Backup & Restore † Create Backup) or iCloud Backup (auto if enabled).

**Q: What banks are supported?**
A: All banks that send transaction SMS. Optimized for Indian banks but works globally.

---

##  Report a Bug

### Via Email
**Email:** numanmubarak@protonmail.com
**Subject:** "Spender Beta Bug Report"

**Please Include:**
- Device model (e.g., iPhone 14 Pro)
- iOS version (e.g., iOS 17.1)
- App version (Settings † About)
- Bug description (what happened vs. expected)
- Steps to reproduce
- Screenshots (if applicable)

**Example Bug Report:**
```
Device: iPhone 13
iOS: 17.0
App Version: 1.0.35

Bug: Account balance shows incorrect amount after editing transaction

Steps to Reproduce:
1. Open account "HSBC Savings"
2. Edit any transaction amount
3. Save transaction
4. Balance doesn't update

Expected: Balance should update immediately
Actual: Balance stays the same until app restart

Screenshot: [attached]
```

---

##  Feature Requests

We'd love to hear your ideas!

**Email:** numanmubarak@protonmail.com
**Subject:** "Spender Beta Feature Request"

**Tell Us:**
- What feature you'd like
- Why it would be useful
- How you'd use it in your daily workflow

---

##  Additional Resources

- **App Homepage:** [README.md](README.md)
- **Privacy Policy:** [PRIVACY_POLICY.md](PRIVACY_POLICY.md)
- **App Store:** [Download Spender Beta](README.md#installation)
- **Email Support:** numanmubarak@protonmail.com

---

##  Checklist for Common Issues

### SMS Not Working?
- [ ] SMS Analyzer downloaded (Settings † SMS Analyzer)
- [ ] SMS Automation enabled (Settings † Automation)
- [ ] iOS Shortcut created (Settings † Automation † Setup Shortcut)
- [ ] SMS permissions granted (iOS Settings † Spender)
- [ ] Bank SMS format is standard transaction notification

### Balance Wrong?
- [ ] Starting balance set correctly
- [ ] No duplicate transactions
- [ ] All transactions assigned to correct account
- [ ] Account merges completed (if applicable)

### Backup Not Working?
- [ ] Sufficient storage space (local or iCloud)
- [ ] iCloud signed in (for iCloud backup)
- [ ] iCloud Drive enabled (for iCloud backup)
- [ ] Stable internet connection

### Can't Import CSV?
- [ ] CSV has required columns (Date, Amount, Description)
- [ ] Date format is recognizable
- [ ] Amount format is numeric (no currency symbols)
- [ ] File encoding is UTF-8

---

##  Thank You

Thank you for using Spender Beta! Your feedback helps us build the best privacy-focused finance app.

**Happy tracking!** 

---

*Last Updated: November 22, 2025*

*For app updates, check the App Store or your email for beta announcements.*
