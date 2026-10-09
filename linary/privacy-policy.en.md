---
title: "Privacy Policy — Linary"
---

# Privacy Policy — Linary

**Effective date:** 9 October 2026

Linary is a "one line" puzzle: draw a line from 1 through every number in order, visiting each cell exactly once. The app has a daily puzzle with a streak and a calendar, the chapters of the Path, a timed Rush and an endless mode. This policy explains what data the app uses and how it handles it.

**In short: Linary has no accounts, no server of its own and no analytics. Your progress is stored on your device. The app is free because it shows ads: they are served by the Yandex Advertising Network, and the Yandex module built into the app receives information about your device (section 5). Apart from ads, the app goes online only to check today's date (section 4).**

## 1. Who processes the data

Developer: kotdikii.
Contact for privacy questions: **kotdikii@gmail.com**

## 2. What the app collects

Linary itself **collects no personal data**: it does not ask for your name, email or phone number, creates no account and uses no analytics. The app has no server of its own, so none of your data is sent to the developer at all.

The app's private folder on your device holds:

- **progress**: solved daily puzzles (the day, the solving time and whether a hint was used), your day streak and streak freezes, completed chapter levels, the count and best time in endless mode, your Rush record;
- **settings**: language, theme, palette, sound, vibration, line style, your answer about personalised ads;
- **crash reports** (section 7).

The data the Yandex ad module receives is described in section 5. The app does not pass your progress to it, only what is needed to show ads.

## 3. Permissions

| Permission | Why it is needed |
|---|---|
| Internet | Loading ads and checking today's date (section 4) |
| Network state | The ad module checks for a connection before loading a video |
| Advertising ID | Required by the Yandex ad module (section 5) |
| Install referrer | The ad module asks Google Play where the app was installed from |

The app asks for no other permissions. In particular:

- **Location is not requested.** To decide whether it has to ask for consent to personalised ads (section 5), the app looks at the country of your mobile network, SIM card or system language. This is done on the device and is not sent anywhere.
- **Files, contacts, camera and microphone are not requested.**
- Vibration on line steps uses the system's haptic feedback and needs no separate permission.

## 4. Date check

The daily puzzle is the same for everyone and changes at midnight, and the streak counts days. So that changing the phone's clock cannot unlock tomorrow's puzzles or repair a broken streak, the app checks the current date online: it sends a header request (HEAD) to `https://ya.ru` or `https://www.google.com` and takes **only the date** from the response.

The request carries nothing about you or your game. The server sees only what it sees with any connection: an IP address and the client type. The checked date is kept on the device until the phone restarts. Without a connection the daily puzzles do not open, and the rest of the game works.

## 5. Ads

The app is free and is paid for by ads. They are served by the **Yandex Advertising Network**, whose module (SDK) is built into the app.

**What kinds of ads there are.**

- **Rewarded videos.** Watching them is up to you. A video watched to the end gives a hint (the first hint in every puzzle is free), a one-day try-on of a locked line style, or a streak freeze. A video is shown only when you tap.
- **Full-screen ads** between puzzles: after several solved endless-mode puzzles or Path levels, and after a Rush. They are not shown on the first launch, right after a rewarded video, or in the middle of a puzzle.

**What the ad module receives.** To choose and show ads, the Yandex module receives from the device: the Android advertising ID, the device model and system version, the language, the network type, the IP address (which gives an approximate region), the app's install source, and information about ad impressions and taps. This data is processed by **Yandex** under its own rules:

- [Yandex Privacy Policy](https://yandex.com/legal/confidential/)
- [Yandex Advertising Network SDK Terms of Use](https://yandex.com/legal/mobileads_sdk_agreement/)

The developer does not receive this data. The only thing the app learns from the module is whether a video was watched to the end, so that it can give the reward.

**Personalised ads.**

- **In the European Economic Area, the United Kingdom and Switzerland**, the app asks on first launch whether ads may be personalised. Your answer does not affect the game. Without your consent ads are still shown, but they are not personalised. You can change your answer at any time: Settings → Personalised ads.
- **In other countries**, personalised ads are controlled in the Android settings: Settings → Privacy (or Google) → Ads. There you can reset or delete your advertising ID.

## 6. Sharing a result

After solving the daily puzzle you can share your result: the puzzle number, level, time and streak. This happens **only when you tap**: the text goes to the system Share sheet, and you choose the recipient. The text does not contain the solution.

## 7. Crash reports

If the app crashes or freezes, it writes a technical report (error details, app version and device model) **to a file on your device**. Reports are shown under About → Crash reports.

**They are never sent automatically.** You can send a report only by hand: tap an entry and choose how to send it. The list of reports can be cleared at any time.

## 8. System backup

If Android backup is turned on in your device settings, the system may copy the app's progress and settings to your Google account and move them to a new phone under its own rules. Crash reports are not included. This process is controlled by the operating system, not by the app.

## 9. Storage and deletion

All of the app's data lives in its private folder on the device. **Uninstalling the app erases it completely**: progress, streak, settings and crash reports. You can also clear the data with Android: Settings → Apps → Linary → Storage.

The data received by the ad module is stored and deleted by Yandex under its own policy (section 5).

## 10. Children

The app is not intended for children under 13. The ad module it uses is not designed for a child audience.

## 11. Changes to this policy

If the policy changes, we will update the text and the effective date on this page.

## 12. Contact

For any privacy questions: **kotdikii@gmail.com**
