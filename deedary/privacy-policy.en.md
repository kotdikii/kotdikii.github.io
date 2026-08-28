---
title: "Privacy Policy — Deedary"
---

# Privacy Policy — Deedary

**Effective date:** 28 August 2026

Deedary is a personal kanban board: columns and tasks, checklists, due dates with reminders, time tracking and statistics. This policy explains what data the app uses and how it handles it.

**In short: Deedary has no accounts, no server of its own, no ads and no analytics. Your boards, tasks and time entries are stored on your device only. Without an explicit action from you, the app does not go online at all.**

## 1. Who processes the data

Developer: kotdikii.
Contact for privacy questions: **kotdikii@gmail.com**

## 2. What the app collects

Deedary **collects no personal data**: it does not ask for your name, email or phone number, does not create an account, shows no ads and uses no analytics. The app has no server of its own, so there is simply nowhere for your data to be sent.

Everything you create in the app — boards, folders, columns, tasks, notes, checklists, labels, due dates, repeat rules, time entries, the archive and settings — is stored **on your device**, in the app's private directory.

## 3. Permissions

| Permission | Why it is needed |
|---|---|
| Notifications | Reminders about task due dates and the running timer notification |
| Start after reboot | To re-arm reminders: system alarms do not survive a device restart |
| Internet | **Only** for a cloud backup — if you have connected one |

The app requests no other permissions. In particular:

- **No file access permission is requested.** A backup is saved and read through the system file picker, which grants access only to the file you pointed at.
- **No exact alarms are requested.** Reminders are scheduled the ordinary way, and the system may shift them by a few minutes to save battery.
- The notification permission is requested **not at first launch** but when you switch on your first reminder. Without it the app works fully, only silently.

## 4. Third-party services

**By default, none.** The app contacts no network service: not for data, not for images, not for update checks. The Internet permission stays unused until you connect a cloud backup.

The only external services the app may contact are the **cloud storages you connect yourself** (section 5).

## 5. Backup

A backup is a single JSON file holding your data: boards, folders, columns, tasks, checklists, labels, repeat rules, time entries, the archive and settings. It is created and restored **only on your command**.

**Saving to a file.** The location is chosen through the system dialog; the app does not remember the path and has no access to your other files.

**Saving to a cloud (optional).** Yandex Disk and Google Drive are supported. Signing in happens on those services' own pages; **the app never sees or stores your password**. The permissions requested are the narrowest available:

| Service | Scope | What it grants |
|---|---|---|
| Yandex Disk | `cloud_api:disk.app_folder` | Access **only to the app's own folder** on your Disk |
| Google Drive | `drive.file` | Access **only to the files the app itself created** |

These scopes do not let the app read your other files, photos or documents — it cannot see them. The app does not request your login, name or email address in the cloud account.

The access token issued by the service is kept in the app's private storage on the device and is deleted together with the app; the "Disconnect" button erases it immediately. You can also revoke access on the service side, in the security settings of your Yandex or Google account.

**Signing in to Google happens in one of two ways**, depending on the device: through Google Play services when they are present, or by entering a code at `google.com/device` when they are not. The set of requested permissions is the same either way.

In addition, **Android system backup** applies: if it is enabled in your device settings, Android may copy the app's data to your cloud account under its own rules. That process is controlled by the operating system, not by the app.

## 6. Report and table export

The statistics screen can hand you a report for the period as text and export time entries as a CSV table. Both happen **only when you tap the button**: the text goes to the system "Share" dialog where you pick the recipient, and the table is saved to a file through the system dialog. Nothing is sent anywhere on its own.

## 7. Crash reports

If the app crashes or freezes, it writes a technical report (error details, app version and device model) **to a file on your device**. Reports are listed under "About" → "Crash reports".

**They are never sent automatically.** A report can only be sent manually, by tapping an entry and choosing how to send it. The list can be cleared at any time.

## 8. Storage and deletion

All app data lives in its private directory on the device. **Uninstalling the app erases it completely** — boards, tasks, time entries, settings and cloud access tokens. You can also clear the data through Android ("Settings" → "Apps" → Deedary → "Storage").

Backup files you saved yourself are not removed when the app is uninstalled — they stay where you put them (in a file or in your cloud), and they are yours to manage.

## 9. Children

The app is not intended to collect data from children and collects no personal data at all.

## 10. Changes to this policy

If the policy changes, we will update the text and the effective date on this page.

## 11. Contact

For any privacy questions: **kotdikii@gmail.com**
