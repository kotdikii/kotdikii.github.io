---
title: "Privacy Policy — Seriary"
---

# Privacy Policy — Seriary

**Effective date:** August 4, 2026

Seriary is an app that picks a random episode from your favourite TV shows and helps you open it in a streaming service. This policy explains what data the app uses and how it is handled.

**In short: Seriary has no accounts, no server of its own, no ads and no analytics. Your library, watch marks and history are stored on your device only. The app goes online solely for show metadata and posters — and only when you ask it to.**

## 1. Who processes the data

Developer: kotdikii.
Privacy contact: **kotdikii@gmail.com**

## 2. What data the app collects

Seriary **does not collect personal data**: it never asks for your name, email or phone number, creates no account, shows no ads and uses no analytics. The app has no backend of its own, so there is nowhere for your data to be sent.

Everything you create in the app — your list of shows, folders, watch marks, favourites, excluded episodes, roll history and settings — is stored **on your device**, in the app's private storage.

## 3. Permissions

| Permission | Why it is needed |
|---|---|
| Internet | Searching for shows, downloading season and episode data, posters |
| Network state | Checking whether a connection exists before going online |

The app requests no other permissions. In particular, **no storage permission is requested**: saving and reading a backup uses the system file picker, which grants access only to the one file you point at.

## 4. Third-party services the app contacts

The app needs show metadata and takes it from open sources. None of them requires registration or an API key, so you are an anonymous visitor to them. As with any request to a website, these services can see your IP address — without it there would be nowhere to send the reply.

| Service | What is sent | When |
|---|---|---|
| MyShows (`api.myshows.me`) | Search query, show identifier | When searching, adding a show, or refreshing its data |
| TVmaze (`api.tvmaze.com`) | Show identifier | At the same time — for episode runtimes and descriptions |
| Kinopoisk (`st.kp.yandex.net`, `avatars.mds.yandex.net`) | A request for a poster image | When covers are displayed. This is static image hosting; the app does not call the Kinopoisk API |
| MyMemory (`api.mymemory.translated.net`) | **The text of an episode or show description** | Only when you tap "Translate" — see section 5 |

None of these requests carries information about you, your device, or your library as a whole — only what is needed for that particular reply.

## 5. Translating descriptions

The sources provide episode descriptions in English only. The "Translate" button sends **the description text** to the MyMemory machine-translation service and receives the translation back. The result is stored on your device so it never has to be requested twice.

Translation **never happens on its own** — only when you tap the button. If you do not use it, the app never contacts that service at all. MyMemory's own terms are available on its website; note that the text you send is processed on their side.

## 6. Backup

A backup is a single file into which the app writes your library: shows, seasons and episodes, watch marks, favourites, folders, roll history, stored translations and settings. It is created and restored **only on your command**.

**Saving to a file.** You choose the location through the system dialog; the app does not remember the path and has no access to any of your other files.

**Saving to the cloud (optional).** Yandex Disk and Google Drive are supported. Sign-in happens on the service's own official page; **the app never sees or stores your password**. The minimum possible scopes are requested:

- Yandex Disk — `cloud_api:disk.app_folder`: access **only to the app's own folder** on your Disk;
- Google Drive — `drive.appdata`: access **only to the app's hidden application-data folder**.

Neither scope lets the app read the rest of your files, photos or documents — it cannot see them. The app does not request your login, name or email address in the cloud account. The access token issued by the service is kept in the app's private storage on your device and is removed together with the app. You can revoke access at any time in the security settings of your Yandex or Google account.

**Android system backup** also applies: if it is enabled in your device settings, Android may copy the app's data to your cloud account under its own rules. That process is controlled by the operating system, not by the app.

## 7. Crash reports

If the app crashes or freezes, it writes a technical report (error details, app version and device model) **to a file on your device**. The reports are listed under "About" → "Crash reports".

**They are never sent anywhere automatically.** A report can only be sent by you, manually, by tapping an entry and choosing how to share it. You can clear the list at any time.

## 8. Opening streaming services

The "Find on …" button opens the page or the app of the service you chose (Kinopoisk, Ivi, Okko, Wink, START, Amediateka, Netflix). When it does:

- the **show title** is placed on the clipboard so that you do not have to type it into that service's search box;
- everything after that happens **on that service's side** and is governed by its own privacy policy.

Seriary is not affiliated with these services, sends them no information about you, and has no access to your accounts or subscriptions there.

## 9. Data storage and deletion

All app data lives in its private directory on the device. **Uninstalling the app erases it completely** — library, marks, history, stored translations, settings and cloud access tokens. You can also clear the data through Android ("Settings" → "Apps" → Seriary → "Storage").

Backup files that you saved yourself are not removed when the app is uninstalled — they stay where you put them and remain under your control.

## 10. Children

The app is not intended to collect data from children and does not collect personal data at all.

## 11. Changes to this policy

If this policy changes, we will update the text and the effective date on this page.

## 12. Contact

For any privacy questions: **kotdikii@gmail.com**
