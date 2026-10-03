# Privacy Policy for Life & Lessons (Quotes App)

**Effective Date:** October 3, 2026  
**Last Updated:** October 3, 2026  
**Application Name:** Life & Lessons (formerly Quotes App)  
**Package Name:** `com.lifeandlessons.app`  
**Developer:** Tarun Shukla  
**Contact Email:** [tarunshukla913@gmail.com](mailto:tarunshukla913@gmail.com)  
**Repository:** [https://github.com/tarunshukla11/turtlecode1](https://github.com/tarunshukla11/turtlecode1)  

---

## 1. Overview & Core Philosophy

**Life & Lessons** is a mobile and web application designed to offer daily perspective, timeless thoughts, inspirational wisdom, customized wallpapers, and native Android home screen widgets.

Our core commitment to our users is simple: **Privacy-First and Offline-First**.

- We **do not** collect any personally identifiable information.
- We **do not** require you to create an account or sign in.
- We **do not** sell, rent, or share your data with any third parties or advertisers.
- All your quote favorites, shuffle histories, and settings remain stored **locally on your device**.

---

## 2. Information We Collect (Or Rather, Do NOT Collect)

### 2.1 Personal Data
We do not collect, request, store, or transmit any personal data, including but not limited to:
- Name, username, or age
- Email address or phone number
- Physical address or location data
- Device identifiers (IMEI, MAC address, Advertising ID)
- Payment information or financial details

### 2.2 Local Storage & Device Data
The app functions 100% offline using a built-in library of curated thoughts. The following data is stored solely on your local device (using Android `SharedPreferences` and browser `localStorage`):
- **Favorite / Saved Quotes:** Quotes you mark with a heart.
- **Seen History / Shuffle Memory:** Quote IDs you have recently viewed, ensuring quotes do not repeat consecutively.
- **Preferences:** Your selected theme (Gold, Aurora, Minimal, Sunset, Emerald), preferred font style, and preferred daily reminder time.
- **Wallpaper Settings:** Your chosen frequency (Daily, Every 3 days, Weekly, or Screen-Lock mode) and screen target (Home, Lock, or Both).

**None of this information is ever uploaded or transmitted to any external server.**

---

## 3. Android Permissions & Why They Are Requested

The Android version of Life & Lessons requests only the minimal permissions necessary to deliver its core native features:

| Permission | Android Identifier | Purpose / Usage |
| :--- | :--- | :--- |
| **Set Wallpaper** | `android.permission.SET_WALLPAPER` | Allows you to apply wisdom quote wallpapers to your Home Screen, Lock Screen, or Both. Also used when you choose to enable automatic daily or screen-lock wallpaper updates. |
| **Receive Boot Completed** | `android.permission.RECEIVE_BOOT_COMPLETED` | Restores your scheduled wallpaper update timer and refreshes your Home Screen Widgets after your device restarts. |
| **Post Notifications** | `android.permission.POST_NOTIFICATIONS` | Delivers your daily perspective reminder at your chosen time (if enabled in Settings). We never send marketing, commercial, or spam notifications. |
| **Internet Access** | `android.permission.INTERNET` | Required by the underlying Capacitor / WebView framework. The application contains an embedded local database of 256 quotes and does not make unauthorized outbound requests. |
| **Storage / Media (Legacy)** | `android.permission.WRITE_EXTERNAL_STORAGE` *(API ≤ 28 only)* | Only utilized if you explicitly tap "Export Collection" or save a generated wallpaper image to your local Downloads folder. |

---

## 4. Home Screen Widgets & Screen-Lock Features

### 4.1 Real Native Android Home Screen Widgets
- The app offers Small (2x2), Medium (4x2), and Large (4x3) Android Home Screen Widgets.
- Widgets render using native Android `RemoteViews` and pull from the local offline database.
- They do not collect telemetry, track usage, or connect to external analytics.

### 4.2 "Every Time Screen is Locked" Wallpaper Automation
- When you explicitly choose this automation mode in Wallpaper Studio, a lightweight Android background service listens locally for the system screen-off event (`Intent.ACTION_SCREEN_OFF`).
- When your screen turns off, a new eligible local quote is selected and applied as your wallpaper.
- This feature works entirely offline, does not use continuous polling or wake locks, and does not monitor any other user activities.

---

## 5. Third-Party Services and Analytics

- **No Third-Party Trackers:** Life & Lessons does not integrate Google Analytics, Firebase Analytics, Facebook SDK, or any third-party tracking services.
- **No Ads:** The app does not display banner ads, interstitial ads, or video ads. There are no advertising SDKs included in the codebase.

---

## 6. Children's Privacy (COPPA & GDPR Compliance)

Life & Lessons contains positive, educational, and philosophical quotes suitable for general audiences.
- We do not knowingly solicit or collect personal information from children under the age of 13 (or under 16 in the European Union).
- Because no personal data is collected from any user, our application is safe for users of all ages.

---

## 7. Data Retention, Control, and Deletion

You retain full control over your data at all times:
- **Clear Saved Quotes:** You can permanently delete all saved quotes from **Settings → Clear Saved Quotes**.
- **Reset History:** You can clear shuffle memory from **Settings → Reset Shuffle Memory**.
- **Complete Deletion:** Uninstalling the app from your device automatically and permanently purges all local storage, preferences, and cached wallpapers created by the application.

---

## 8. Security

We take the security of your device and data seriously. Because all your preferences and saved thoughts remain on your device within the app's sandboxed private storage, your information is protected by Android's security architecture. No data travels over public networks.

---

## 9. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in app functionality or legal requirements. Any modifications will be committed to this repository with an updated "Last Updated" date. We encourage you to review this policy periodically.

---

## 10. Contact Us

If you have questions, suggestions, or concerns regarding this Privacy Policy or the privacy practices of Life & Lessons, please contact:

- **Developer:** Tarun Shukla
- **Email:** [tarunshukla913@gmail.com](mailto:tarunshukla913@gmail.com)
- **GitHub Repository:** [https://github.com/tarunshukla11/turtlecode1](https://github.com/tarunshukla11/turtlecode1)
