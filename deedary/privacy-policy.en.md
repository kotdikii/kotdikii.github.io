---
title: "Privacy Policy — Deedary"
---

# Privacy Policy — Deedary

**Effective date:** 8 September 2026

Deedary is a kanban board on your phone: columns and tasks, checklists, due dates with reminders, time tracking and statistics. A board can be opened up to other people through your Google Drive. This policy explains what data the app uses and how it handles it.

**In short: Deedary has no accounts, no server of its own, no ads and no analytics. Your boards, tasks and time entries are stored on your device. Data leaves the device in two ways only, and you switch on both of them yourself: a cloud backup (section 5) and shared boards (section 6).**

## 1. Who processes the data

Developer: kotdikii.
Contact for privacy questions: **kotdikii@gmail.com**

## 2. What the app collects

Deedary **collects no personal data**: it does not ask for your name, email or phone number, does not create an account of its own, shows no ads and uses no analytics. The app has no server of its own, so there is simply nowhere for your data to be sent.

Everything you create in the app — boards, folders, columns, tasks, notes, checklists, labels, due dates, repeat rules, time entries, the archive and settings — is stored **on your device**, in the app's private directory.

The exceptions are the cloud backup (section 5) and shared boards (section 6). In both cases the data goes **to storage you chose, by an action you took** — not to the developer, who still has none of it.

## 3. Permissions

| Permission | Why it is needed |
|---|---|
| Notifications | Reminders about task due dates and the running timer notification |
| Start after reboot | To re-arm reminders: system alarms do not survive a device restart |
| Exact alarms | So that a reminder arrives at the minute you set |
| Internet | **Only** for a cloud backup and shared boards — if you have connected them |

The app requests no other permissions. In particular:

- **No file access permission is requested.** A backup is saved and read through the system file picker, which grants access only to the file you pointed at.
- **No contacts permission is requested.** You type a board member's address yourself; your address book is not available to the app.
- **Exact alarms are optional.** The permission is requested when you switch on your first reminder. If you decline it, or revoke it later, the app falls back to an ordinary alarm and the system may then shift the reminder to save battery.
- The notification permission is requested **not at first launch** but when you switch on your first reminder. Without it the app works fully, only silently.

## 4. Third-party services

**By default, none.** The app contacts no network service: not for data, not for images, not for update checks. The Internet permission stays unused until you connect a cloud backup or shared boards.

The only external services the app may contact are the **cloud storages you connect yourself**: Yandex Disk and Google Drive (sections 5 and 6).

## 5. Backup

A backup is a single JSON file holding your data: boards, folders, columns, tasks, checklists, labels, repeat rules, time entries, the archive and settings. It is created and restored **only on your command**.

**Saving to a file.** The location is chosen through the system dialog; the app does not remember the path and has no access to your other files.

**Saving to a cloud (optional).** Yandex Disk and Google Drive are supported. Signing in happens on those services' own pages; **the app never sees or stores your password**. The permissions requested are the narrowest available:

| Service | Scope | What it grants |
|---|---|---|
| Yandex Disk | `cloud_api:disk.app_folder` | Access **only to the app's own folder** on your Disk |
| Google Drive | `drive.file` | Access **only to the files the app itself created**, plus those you picked yourself in Google's own dialog |

These scopes do not let the app read your other files, photos or documents — it cannot see them. Your cloud login and password are never available to the app; the name from your Google Drive profile is requested only for shared boards (section 6), and only there.

The access token issued by the service is kept in the app's private storage on the device and is deleted together with the app; the "Disconnect" button erases it immediately, and for Google it also revokes the consent itself rather than merely forgetting it. You can also revoke access on the service side, in the security settings of your Yandex or Google account.

**Signing in to Google happens in one of two ways**, depending on the device: through Google Play services when they are present, or by entering a code at `google.com/device` when they are not. The set of requested permissions is the same either way.

In addition, **Android system backup** applies: if it is enabled in your device settings, Android may copy the app's data to your cloud account under its own rules. That process is controlled by the operating system, not by the app.

## 6. Shared boards

A board can be opened up to other people. This is an **optional add-on**: until you connect a Google account and share a board, the app works entirely on the device and everything above holds without qualification. Personal boards never become shared on their own and go nowhere.

**Where a shared board lives.** In a single file, `Deedary · <board name>.jsonl`, on the Google Drive of the **owner** — the person who shared the board; the folder is the same one that holds the backup. There is no server in between: members read and write that file directly, and the developer has no access to it.

**What goes into the board file.** The board's name and colour, its columns and the people assigned to them, tasks with their notes, due dates and priority, checklists, labels, repeat rules, waiting markers, finished time entries and deletion markers. All of it is visible to **every member of the board** — that is what sharing means. Do not put anything there you are not prepared to show the people you invited.

**What never goes there.** Your reminders, the timer running right now, collapsed columns, your folders and the order of boards in your list, app settings, crash reports and, of course, your personal boards.

**Your name.** So that the board can show who picked up a task, the app asks Google Drive for **the name in your profile** and writes it into the board file. Your email address is not written into the board file.

**Inviting and revoking.** You type a member's address, and the app hands it to Google Drive as a permission on the file; the invitation email is sent by **Google itself** — the app has no mailing of its own and never will. The app keeps **no member list**: the "Members" dialog shows what Drive returned (address, name and role) and stores none of it. "Revoke" removes the permission on Drive's side.

**Connecting someone else's board.** The file is chosen through the Google Picker dialog; the picker page at `kotdikii.github.io/deedary/picker.html` is part of this same site, talks to Google only and stores nothing. The app gets access to exactly the one file you picked and sees no other file on that Drive.

**What to understand up front.** The board file sits on the owner's Drive and answers to the owner: they can revoke your access or delete the file, and the board will stop updating — whatever already reached your device stays with you. Exchange happens when you open the app or the board, or pull the board down: the app does not run in the background and promises no instant updates.

## 7. Report and table export

The statistics screen can hand you a report for the period as text and export time entries as a CSV table. Both happen **only when you tap the button**: the text goes to the system "Share" dialog where you pick the recipient, and the table is saved to a file through the system dialog. Nothing is sent anywhere on its own.

## 8. Crash reports

If the app crashes or freezes, it writes a technical report (error details, app version and device model) **to a file on your device**. Reports are listed under "About" → "Crash reports".

**They are never sent automatically.** A report can only be sent manually, by tapping an entry and choosing how to send it. The list can be cleared at any time.

## 9. Storage and deletion

All app data lives in its private directory on the device. **Uninstalling the app erases it completely** — boards, tasks, time entries, settings and cloud access tokens. You can also clear the data through Android ("Settings" → "Apps" → Deedary → "Storage").

Files that already went to a cloud are not removed when the app is uninstalled: your backup stays where you put it, and a shared board's file stays on its owner's Drive together with whatever you contributed to it. Your own backup is yours to manage; the board file is the owner's, and deletion requests go to them.

## 10. Children

The app is not intended to collect data from children and collects no personal data at all.

## 11. Changes to this policy

If the policy changes, we will update the text and the effective date on this page.

## 12. Contact

For any privacy questions: **kotdikii@gmail.com**
