# Privacy Policy — Delivery & Ride Quick Offer

**Effective date:** [FILL IN WHEN PUBLISHED]
**Last updated:** September 15, 2026

Losget Press ("we," "us," or "our") operates the Delivery & Ride Quick Offer mobile application (the "App"). This Privacy Policy explains what information the App collects, how it is used, and your choices.

## Summary (plain language)

- The App does not require you to create an account or sign in.
- Your Offer Rules, Platform Setup preferences, and any location notes you create (Reject / Warning / Rating) are stored **only on your device**. We do not collect them, store them on our servers, or share them with anyone, including other users of the App.
- The only information that leaves your device is: an **anonymous crash report** if the App crashes; basic **app-quality session data** (described below) that our crash-reporting library automatically collects each time you open the App, so Google can calculate crash-rate metrics; and your **subscription purchase status**, which is verified through Google Play (we do not process or see your payment card details — Google handles that).
- We do not sell your data. We do not show ads. We do not use third-party advertising or tracking SDKs.

## What information we collect

### Information you create, stored only on your device
The App stores the following data locally on your device, using standard Android app storage. This data is never transmitted to us, to any other server, or to any other user:
- Offer Rules you configure for each supported platform (minimum pay thresholds, distance limits, etc.)
- Platform Setup preferences and permission status
- Location Reject / Location Warning / Location Rating records you create (approximate coordinates derived from delivery/pickup addresses shown in offer notifications, a radius, a reason, an optional note, and time conditions you set)
- Your selected display language and other app settings
- Your Free-tier usage window status and, if you subscribe, your subscription entitlement status as last confirmed by Google Play

If you uninstall the App, this locally stored data is deleted along with it (standard Android behavior), unless your device's own backup system separately preserves app data.

### Anonymous crash reports
The App uses Firebase Crashlytics to receive anonymous crash and error reports so we can fix bugs. These reports may include technical information such as device model, Android OS version, and the state of the app at the time of the crash. Crash reports are not tied to your name, email, or any account, because the App does not have accounts. Firebase Crashlytics also generates a random installation identifier (a "Crashlytics installation UUID") that identifies an individual app installation — not you personally — so that Google can count how many installations are affected by a given crash.

### App-quality session data (Firebase Sessions SDK)
Firebase Crashlytics automatically includes a component from Google called the Firebase Sessions SDK, which we did not add separately and cannot disable while using Crashlytics. According to Firebase's official documentation, this component automatically collects, on every app open, regardless of whether a crash occurs:
- Basic app metadata: the App's package name, Android OS version, SDK version, and network connection type
- Basic device metadata: device manufacturer and model
- The timestamp when the App is brought to the foreground, which is used to start a new "session"

Google uses this session-timing data to group crashes and performance data into sessions and calculate aggregate metrics such as the percentage of users who experience a crash. This is technical, aggregate app-quality data — it is not a behavioral analytics or advertising profile, and it is separate from the crash report described above (it is collected even on app opens where nothing crashes). We do not use Firebase Analytics, Google Analytics, or any other behavioral-tracking or advertising SDK. (Source: Firebase's official documentation, "Prepare for Google Play's data disclosure requirements," https://firebase.google.com/docs/android/play-data-disclosure, verified September 15, 2026.)

### Subscription purchase status
If you choose to subscribe, purchases are processed entirely by Google Play. We receive confirmation of your subscription status (active, expired, cancelled) from Google Play Billing so the App knows whether to unlock full features. We do not receive or store your payment card number or other payment details — that information is handled by Google. Google's own privacy policy governs how Google processes your payment information: https://policies.google.com/privacy

### Notification content the App reads
To provide its core function, the App requests Android's Notification Access permission so it can read notifications from the supported gig-work platform apps (Uber, DoorDash, Instacart Shopper, Walmart Spark) that you have installed, in order to detect and score incoming job offers. This processing happens entirely on your device. We do not transmit the content of these notifications to any server, and we do not store the raw notification text beyond what is needed to display the offer to you in the moment.

## Permissions the App requests, and why

| Permission | Why the App needs it |
|---|---|
| Notification Access | Core function — reading gig-platform offer notifications to score them |
| Display over other apps (Overlay) | Showing the offer score popup while another app is in the foreground |
| Foreground Service | Keeping offer monitoring running reliably while you work |
| Post Notifications | Showing the App's own status and offer alerts |
| Vibrate | Giving a vibration alert for a new offer while Background Watch monitoring is active |
| Internet | Sending anonymous crash reports to Firebase Crashlytics, verifying your subscription status with Google Play Billing, and reverse-geocoding the addresses you type into approximate coordinates for location notes |
| Network state (Access Network State) | Automatically included by the Firebase SDK we use for crash reporting; lets the App check whether the device currently has connectivity before it attempts to send a crash report |
| Google Play Billing | Automatically included by the Google Play Billing library so the App can process subscription purchases through Google Play |

The App does not request access to your contacts, photos, camera, microphone, or precise GPS location.

### Capabilities that do not require an Android permission
Two features are sometimes mistaken for permissions but do not actually require the App to request any Android permission, because they are implemented using APIs that don't need one:
- **Bluetooth audio device detection**: the App checks whether a Bluetooth headset/earpiece is currently connected, using Android's `AudioManager.getDevices()` API, so voice announcements can be routed to it. This does not require any Bluetooth permission.
- **Call Privacy (call-state detection)**: the App checks whether you are currently in a phone call, using Android's `AudioManager.getMode()` API, so it can pause voice announcements during a call. This does not require the `READ_PHONE_STATE` permission, and the App never accesses call content, call logs, or phone numbers.

## What we do not do

- We do not sell or rent your information to anyone.
- We do not show third-party advertising.
- We do not use third-party advertising or behavioral-tracking SDKs.
- We do not share your Offer Rules, location notes, or ratings with other drivers or with the gig platforms themselves.
- We do not require or use an account system for the free tier.

## Data retention and deletion

Locally stored data remains on your device until you delete it yourself (through the App's settings, where provided) or uninstall the App. Anonymous crash reports are retained by Firebase Crashlytics according to Google's standard retention practices for that service.

## Children's privacy

The App is intended for adults performing gig delivery and rideshare work and is not directed at children. We do not knowingly collect information from children.

## Changes to this policy

We may update this Privacy Policy from time to time. If we make material changes, we will update the "Last updated" date above. Continued use of the App after changes take effect constitutes acceptance of the revised policy.

## Contact us

If you have questions about this Privacy Policy, contact us at: **contact@losget.com**

---
*This document is a baseline privacy policy prepared to accurately describe the App's actual data practices as of the date above. It has not been reviewed by an attorney. Before wide public release, Losget Press should have this policy reviewed by legal counsel familiar with applicable state, federal, and international privacy law (e.g., CCPA, GDPR if applicable) to confirm completeness and compliance.*
