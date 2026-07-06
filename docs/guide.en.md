---
title: "User Guide — DeepCheck"
---

DeepCheck is an app for diagnosing your smartphone's hardware: the display, sensors, camera, microphone, speakers, storage, connectivity modules, and more. All testing runs **locally on the device**, with no data sent to the internet.

This guide explains how to use the app and run the tests.

---

## Contents

1. [General principles](#general-principles)
2. [Navigating the app](#navigating-the-app)
3. [The "Components" section](#the-components-section)
4. [List of tests](#list-of-tests)
5. ["Series" mode](#series-mode)
6. [CPU stress test](#cpu-stress-test)
7. [RAM test](#ram-test)
8. [Storage test](#storage-test)
9. [GPU test](#gpu-test)
10. [The "About device" section](#the-about-device-section)
11. [Settings](#settings)
12. [Pro version and free-mode limits](#pro-version-and-free-mode-limits)
13. [Permissions](#permissions)
14. [FAQ](#faq)

---

## General principles

- Most tests are **interactive**: the app shows what to do (tap, swipe, place your finger, listen to a sound, etc.), and you confirm the result — whether the test **passed** or **failed**.
- Each test records a result: ✅ passed or ❌ failed. This helps you see which components are working correctly.
- Before tests that need hardware access (camera, microphone, sensors, storage), the app requests the matching **permission**. Without it, the test will be limited.
- The app does not collect or send any of your data anywhere.

---

## Navigating the app

### Side menu (☰)

Opens via the three-line button in the top-left corner or by swiping from the left edge. It contains the main sections:

- **Components** — a list of 24 individual hardware tests.
- **About device** — detailed information about the phone's hardware and specifications.
- **Stress test** — a CPU load test.
- **RAM test** — a memory benchmark.
- **Storage test** — a storage speed benchmark.

### Overflow menu (⋮)

Opens via the button in the top-right corner. It contains:

- **Settings** — choose theme and language.
- **Help** — opens this guide.
- **About app** — version, features, and developer information.

---

## The "Components" section

This is the main section with individual tests. Pick a test from the list, and the app will walk you through the check step by step.

**How a test runs:**

1. Open a test from the list.
2. Read the instructions on the start screen (what will be checked and how).
3. Start the check and perform the required actions.
4. Confirm the result: if the component works correctly, mark it as **passed**; if there's a problem, mark it as **failed**.

After finishing, you return to the list, where you can see which tests have already been completed and their results.

---

## List of tests

The app includes **24 tests**, grouped by component type.

### Display and touch

- **Display test** — checks color reproduction and looks for dead pixels (fills the screen with solid colors).
- **Touchscreen test** — checks the response across the entire touchscreen area.
- **Multitouch test** — checks simultaneous recognition of multiple touches.
- **Brightness test** — checks backlight brightness control.

### Buttons and biometrics

- **Buttons test** — checks the physical buttons (volume, power, etc.).
- **Fingerprint test** — checks the fingerprint sensor (requires at least one fingerprint enrolled in system settings).

### Sound and vibration

- **Audio test** — checks the speakers.
- **Headset test** — checks a wired/wireless headset.
- **Vibration test** — checks the vibration motor.

### Camera and flash

- **Camera test** — checks the front and rear cameras.
- **Flash test** — checks the LED flash.

### Power and storage devices

- **Charging test** — monitors charging status and parameters.
- **SD card test** — checks the MicroSD slot (a card must be inserted).
- **OTG test** — checks USB-OTG support (an external device must be connected).

### Connectivity

- **NFC test** — checks the NFC module.
- **SIM test** — checks SIM card detection.
- **Wi-Fi test** — checks the Wi-Fi module.
- **Bluetooth test** — checks the Bluetooth module.
- **GPS test** — checks satellite signal reception.

### Sensors

- **Accelerometer test** — checks the acceleration sensor.
- **Gyroscope test** — checks the angular velocity sensor.
- **Magnetometer test** — checks the digital compass.
- **Light sensor test** — checks the ambient light sensor.
- **Proximity test** — checks the proximity sensor (the one that triggers near your ear during a call).

> The set of available tests depends on which modules and sensors your device actually has.

---

## "Series" mode

**Series** mode lets you run several selected tests in a row without returning to the list each time. It's handy for a quick all-around device check (for example, before buying or selling a used phone).

- Select the tests you want and start the series.
- During the series, a control panel appears at the bottom: move to the previous/next test, skip, or finish.
- When the series ends, a summary is generated: which tests passed, failed, were skipped, or weren't completed.

> Series mode is available in the **Pro** version.

---

## CPU stress test

Loads all CPU cores and tracks CPU usage, frequency, and device temperature in real time. It's used to check stability and cooling and to detect throttling (frequency reduction due to overheating).

**Parameters:**

- **Duration** — how long the test runs.
- **Load level** — from gentle to maximum.
- **Load profile:**
  - **Comprehensive** — integer operations, SIMD/FP arithmetic, matrices, and memory together. The default all-purpose mode, close to real-world scenarios.
  - **FPU torch** — maximum load on the floating-point unit. The "hottest" mode; provokes throttling fastest and reveals instability.
  - **Memory** — heavy work on the memory subsystem. Heats the memory controller and checks RAM bandwidth and stability.

**During the test**, load and temperature graphs are shown. If a frequency drop under load is detected, the app will report **throttling detected**.

**Run history** — the results of recent runs are saved so you can compare device behavior at different times or with different settings.

---

## RAM test

A memory benchmark. It measures write, read, and copy speed plus memory access latency. The results help you assess the performance of your device's memory subsystem.

> On some devices the test may run in **limited mode** — this is due to system limits on how much memory can be allocated.

---

## Storage test

A storage speed benchmark: it measures real read and write speeds.

- **Internal storage** is tested for free.
- **External drives** (USB-OTG, SD card) — testing is available in the **Pro** version.

**Clarifying the USB drive version.** When you connect an external drive, the app may offer to grant access to the USB device in order to tell a USB 3.0 drive from a USB 2.0 one when it's plugged into the phone's USB 2.0 port. This is optional — the test will start either way, but the detected specs will be less precise.

> Keep in mind: the real speed may be limited by the device's USB port rather than by the drive.

---

## GPU test

A graphics benchmark for comparing the power of devices using clear metrics — **GFLOPS** and **FPS** — and for checking throttling under sustained load.

The run is **a single continuous stage** under load:

- **GFLOPS** — the GPU's compute performance, measured with a pure compute workload. The same workload heats the GPU up, so from the drop in GFLOPS over time the app detects **throttling** (a frequency drop caused by overheating).
- **3D scene (FPS)** — alongside the GFLOPS load, short probes measure the FPS of a 3D scene (the load is briefly paused so the measurement stays accurate). FPS shows the graphics drop under heat. You can turn the scene off in the test settings, leaving only the GFLOPS measurement.

**Parameters:**

- **Duration** — from 2 to 15 minutes. Runs shorter than 2 minutes aren't saved to history: there's too little data and throttling doesn't have time to appear.
- **Run 3D scene (FPS)** — enable/disable the FPS probes.

The first ~30 seconds run "from cold" to capture peak performance before the GPU heats up. The test runs full-screen with the orientation locked; the device will get noticeably warm. When it finishes you'll see peak and average GFLOPS, FPS, any detected throttling, and the GPU temperature. Results are saved to the **run history**.

> The more powerful the GPU, the higher the GFLOPS and FPS. Results are comparable across devices, but a single synthetic test can't perfectly rank different architectures (e.g. Adreno vs Mali) — that's normal for any benchmark.
> If the device was already hot at the start, the peak and the drop may be understated — let it cool down and restart the test.

---

## The "About device" section

A detailed summary of the phone's hardware: processor, memory, display, cameras, sensors, connectivity modules, Android version, security patch, and other specs. Useful for checking that the device matches its advertised specifications.

---

## Settings

Available from the overflow menu (⋮) → **Settings**:

- **Theme** — light, dark, or system.
- **Language** — the interface language (or the system language).

Settings apply immediately and persist between app launches.

---

## Pro version and free-mode limits

The core tests are free. Some features are part of the **Pro** version:

- **Series mode** — running several tests in a row.
- **Exporting results to PDF.**
- **Testing external drives** (USB-OTG and SD cards). Internal storage is free to test.
- **Unlimited runs** of the stress test, RAM test, storage test, and GPU test (in free mode the number of runs is limited — the same limit applies to each of these tests).
- **Extended duration** for the stress test.

In free mode the app shows how many runs are left. When the limit is reached, you'll be offered an upgrade to Pro.

---

## Permissions

The app requests permissions only to test specific hardware, and **only at the moment** they're needed for the relevant test:

- **Camera** — for the camera and flash tests.
- **Microphone** — for sound/recording checks.
- **Location** — for the GPS test and Wi-Fi scanning.
- **File/storage access** — for the storage test.
- **Bluetooth, NFC, etc.** — for the matching connectivity tests.

If you decline a permission, the test will be limited. You can grant the permission later in the app's system settings.

---

## FAQ

**A test won't start or a module is "not found."**
Most likely your device doesn't have the corresponding hardware module (for example, NFC or a magnetometer), or the required permission wasn't granted.

**Storage speed is lower than expected.**
The real speed can be limited by the device's USB port, the type of connection, or the condition of the drive.

**The stress test shows throttling — is that a defect?**
Not necessarily. Reducing frequency under sustained load is a normal overheating-protection mechanism. Strong, early throttling may indicate cooling problems.

**Where is my data?**
All results and measurements stay on the device. The app does not send data to the internet. See the Privacy Policy for details.

---

*If you still have questions, email the developer: **kotdikii@gmail.com***
