# Privacy Policy for Pocket Ledger

**Effective Date:** November 4, 2024
**Last Updated:** November 4, 2024
**Application Name:** Pocket Ledger
**Package Name:** `in.allbengal.pocketledger`

> [!NOTE]
> Pocket Ledger is designed with a **privacy-first architecture**. Your financial data is stored locally on your device and is never uploaded to any third-party server or developer backend.

---

## 1. Information We Collect and Process

Pocket Ledger is an offline-capable personal expense and income tracker. We do not operate developer servers or sell user data.

### A. Local Financial Data
All financial records, transactions, category names, notes, and monthly budget limits entered into Pocket Ledger are stored locally on your Android device using an encrypted local SQLite database (Android Room) and DataStore Preferences.

### B. Google Account & Drive Integration (Optional)
If you explicitly choose to use the **Google Drive Backup & Restore** feature:
- Pocket Ledger uses standard Google Sign-In (`com.google.android.gms:play-services-auth`) to request restricted access to Google Drive under the `https://www.googleapis.com/auth/drive.file` permission scope.
- **Scope Limitation:** Pocket Ledger can ONLY view, create, and modify backup files created directly by Pocket Ledger inside a dedicated `"Pocket Ledger"` folder on your Google Drive account. Pocket Ledger cannot read or access any other files on your Google Drive.
- No Google account tokens or personal email details are ever sent to the developer or any third party.

---

## 2. How Your Data Is Used

Your data is processed strictly for providing local application functionality:
- Calculating monthly income, expense totals, category breakdowns, and budget spending limits.
- Generating local CSV spreadsheet exports.
- Syncing backup CSV files directly to and from your personal Google Drive storage when requested by you.

We **do not**:
- Collect personally identifiable information (PII).
- Track your usage across other apps or websites.
- Use third-party analytics SDKs, advertising IDs, or telemetry tracking.
- Monetize or sell any user data.

---

## 3. Permissions Used by the Application

| Permission | Purpose |
| :--- | :--- |
| `INTERNET` | Required exclusively for communicating directly with Google Drive APIs when performing cloud CSV backup or restoration. |
| `ACCESS_NETWORK_STATE` | Required to check network availability before initiating Google Drive sync. |

---

## 4. Data Sharing and Disclosure

Because we do not store your data on external servers, we have no access to your data and cannot disclose or sell it to any third party, advertiser, or data broker under any circumstances.

If you choose to use Google Drive backup, your data is transferred securely via HTTPS directly between your device and Google LLC servers, governed by [Google's Privacy Policy](https://policies.google.com/privacy).

---

## 5. Data Retention and Deletion

You retain full ownership and control over all your data at all times:
- **Local Data Deletion:** You can delete individual transactions, clear specific date ranges via **Settings > Clear Selective Records**, or erase all local app data instantly via **Settings > Reset App Data**.
- **App Uninstall:** Uninstalling Pocket Ledger removes all local SQLite database records and DataStore preferences from your device.
- **Google Drive Backups:** You can view, manage, or delete backup CSV files at any time by logging into your Google Drive account (`https://drive.google.com/`) and navigating to the `"Pocket Ledger"` folder.

---

## 6. Children's Privacy

Pocket Ledger does not target or knowingly collect data from children under the age of 13. The app contains no advertisements, in-app purchases, or social networking features.

---

## 7. Changes to This Privacy Policy

We may update this Privacy Policy periodically. Any updates will be reflected on this page with a revised "Last Updated" date.

---

## 8. Contact Us

If you have any questions or concerns regarding this Privacy Policy or your data privacy in Pocket Ledger, please contact us at:

- **Developer:** All Bengal
- **Package:** `in.allbengal.pocketledger`
