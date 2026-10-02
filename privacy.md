# Spreach – Privacy Policy

*Last updated: October 2, 2026*

Your privacy matters. This Privacy Policy explains what information Spreach (the iOS app) and the Spreach Desktop Companion (the optional computer app) handle, where that information goes, and how you can control it.

---

## 1. Overview

Spreach is designed with privacy in mind. Text‑to‑speech generation runs **on your own devices**, either on your iPhone or, if you choose, on your own computer through the Desktop Companion. Spreach does not operate servers that receive your text, audio, or personal information, and we (the developer) never receive that content.

A few features connect to something outside your iPhone. They are described in detail below:

* **Web articles:** when you enter a URL, your device loads that web page directly from the website.
* **Desktop Companion:** if you use it, your iPhone sends text to your own computer over your local network.
* **App Store:** purchases and purchase verification are handled by Apple.
* **Legal documents:** the Terms of Use and this Privacy Policy are loaded from GitHub when you open them in the app.

---

## 2. Information We Do Not Collect

Spreach and the Desktop Companion do **not**:

* Collect your name, email address, or other account information. No Spreach account is required.
* Send your text, documents, images, or generated audio to the developer or to any Spreach server.
* Track usage analytics or crash analytics.
* Use third‑party trackers or advertising SDKs.
* Sell or share your information with anyone.

---

## 3. Information Stored on Your iPhone

To provide its features, Spreach stores the following **locally on your iPhone**:

* **Reading history:** the text you convert, split into pages, along with the input type, the time it was added, and your last reading position. For web articles, this includes the URL you entered and the text extracted from the page.
* **Audio cache:** generated audio and word‑timing data, so you can replay content without regenerating it.
* **Settings:** your selected voice, speed, theme, text size, and Desktop Companion preference.
* **Trial start date:** stored in the iOS Keychain (see Section 9).

This information is not transmitted to us. Like other app data, it may be included in your device backups (for example, iCloud Backup) depending on your iOS settings. You can delete your reading history, audio cache, and settings at any time from the app's Settings, or by deleting the app.

---

## 4. Documents, Camera, and Photos

* **Documents:** PDF, EPUB, and text files you choose are read and parsed on your device.
* **Camera:** if you choose to scan pages, Spreach uses the camera to capture images. Text is recognized on your device using Apple's Vision framework.
* **Photos:** images you select through the system photo picker are processed the same way. Spreach only receives the images you pick and does not have access to the rest of your photo library.

Captured and selected images are used only to extract text. Spreach keeps the extracted text in your reading history and does not upload the images.

---

## 5. Web Articles (URL Import)

When you enter a web address, Spreach opens that page in a hidden in‑app web view (Apple's WebKit) and extracts its readable text on your device. Please be aware:

* **Your device connects directly to the website.** As with any web browser, the website and its service providers receive your IP address, device and browser information, and the address of the page you requested.
* **The page's own code runs.** Web pages can contain their own scripts, analytics, advertising, and tracking technologies. These are controlled by the website, not by Spreach, and they may run while the page loads.
* **Cookies and website data.** The website may set cookies or store other website data in the app's web view, which WebKit may keep between visits.
* **What Spreach keeps.** Spreach saves the URL and the extracted text in your local reading history (Section 3). It does not send either to the developer.

Your use of a website is governed by that website's own terms and privacy policy. Spreach does not control, and is not responsible for, the privacy practices of websites you choose to open.

---

## 6. Desktop Companion

The Desktop Companion is an optional app for your computer that lets your iPhone use the computer's processor or graphics card to generate audio. It is available to Spreach Premium users and is only used when you turn it on.

**6.1 Discovery on your local network**

* On your iPhone, Spreach asks for iOS **Local Network** permission so it can find the Desktop Companion using Bonjour (mDNS).
* While its service is running, the Desktop Companion announces itself on your local network. This announcement includes the service name, your computer's **host name**, its **local IP address**, and the port number. **Any device on the same network can see it.**

**6.2 Information sent from your iPhone to your computer**

When the Desktop Companion is connected and enabled, your iPhone sends it:

* The text to be spoken, in small segments, along with the selected voice, speed, and a randomly generated request ID.
* Your **signed App Store transaction** for Spreach Premium, so the Desktop Companion can confirm you own Premium. This is Apple's signed record of the purchase. It includes details such as the transaction ID, the product and app identifiers, and the purchase date. It does **not** include your name, Apple ID email address, or payment details.

The computer sends the generated audio back to your iPhone. This traffic stays on your local network between your own devices and is not sent to the developer.

**6.3 Information stored on your computer**

The Desktop Companion keeps a local database file (generations.db) in the same folder as the application. This file may contain:

* **Verified purchase records:** the transaction ID from your App Store purchase, so it does not need to re‑verify the purchase on every request.
* **Saved generations:** for batch requests, the text segments sent from your iPhone and the resulting audio.

This data stays on your computer until you delete it. You can clear it at any time with **Clear Saved Audios** in the Desktop Companion's settings menu, or by deleting the database file.

**6.4 Purchase verification**

The Desktop Companion verifies your purchase **on your computer**, using Apple's cryptographic signature and Apple's public root certificate that is bundled with the app. It does not send your purchase information to Apple, to the developer, or to anyone else.

**6.5 Model and voice downloads**

When it first runs, the Desktop Companion's speech components may download model configuration and voice files from Hugging Face, a third‑party model hosting service. That download is subject to Hugging Face's terms and privacy policy, and Hugging Face may receive your computer's IP address and standard request information. No text or audio is sent as part of this download.

**6.6 Network security**

Depending on the version of the Desktop Companion, communication between your iPhone and your computer may not be encrypted. While the service is running, it accepts connections from other devices on the same network. For these reasons:

* Only run the Desktop Companion on a private network you trust, such as your home network. Do not run it on public or shared Wi‑Fi.
* Shut down the service from the Desktop Companion window or system tray when you are not using it.
* Do not expose the Desktop Companion's port to the internet (for example, through port forwarding).

---

## 7. Device Permissions

Spreach may request the following permissions on iOS:

* **Camera:** to scan printed pages and convert them to text.
* **Local Network:** to discover and connect to the Desktop Companion on your computer. This is only needed if you use the Desktop Companion.

Spreach also uses iOS background audio so playback can continue when the app is in the background. Spreach does not use your microphone, location, or contacts.

You can grant or revoke these permissions at any time in iOS Settings.

---

## 8. In‑App Purchases

When you purchase Spreach Premium through the App Store:

* Payment processing is handled entirely by Apple.
* Spreach does not collect, process, or store your payment information.
* Purchases are verified on your iPhone using Apple's StoreKit 2 framework.
* If you use the Desktop Companion, your signed transaction is also shared with your own computer for verification, as described in Section 6.

---

## 9. Trial Information

When you start your 30‑day free trial, the trial start date is stored **locally on your device** in the iOS Keychain. This information:

* Remains on your device and is not sent to any external server.
* Is used only to determine trial eligibility.
* May remain on your device after you delete the app or use "wipe all data", because iOS keeps Keychain items separately from app data. This prevents the trial from restarting.

---

## 10. Third‑Party Services

Spreach does not include third‑party analytics, advertising, or cloud processing services. The Kokoro 82M speech model is packaged with the iOS app and runs locally. Depending on the features you use, you may interact with these third parties:

* **Apple:** App Store purchases, StoreKit, and iOS services are subject to Apple's Privacy Policy.
* **GitHub:** the Terms of Use, this Privacy Policy, and voice samples are hosted on GitHub. When you open these documents in the app, they are downloaded from GitHub (raw.githubusercontent.com), which may receive your IP address and standard request information under GitHub's Privacy Statement.
* **Websites you open:** see Section 5.
* **Hugging Face:** model and voice file downloads by the Desktop Companion. See Section 6.5.

---

## 11. Data Security and Retention

Spreach does not transmit your content to the developer, which minimizes risk. Information described in this policy stays on your iPhone or your computer, under your control, until you delete it:

* **iPhone:** delete individual items from your history, use "wipe all data" in Settings, or delete the app.
* **Computer:** use **Clear Saved Audios** in the Desktop Companion, or delete the application and its generations.db file.

Trial start dates stored in the iOS Keychain benefit from Apple's hardware‑level security protections. You are responsible for securing your own devices and network, especially when using the Desktop Companion (see Section 6.6).

---

## 12. Children's Privacy

Spreach does not knowingly collect personal data from children. If you believe information has been inadvertently collected, contact us immediately.

---

## 13. Policy Changes

We may update this Privacy Policy from time to time. Any changes will be reflected within the app or on spreach.app, and the "Last updated" date above will change.

---

## 14. Contact

If you have questions about this Privacy Policy:
**Website:** [https://spreach.app](https://spreach.app)
