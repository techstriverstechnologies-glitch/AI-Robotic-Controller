# AI Robotic Controller — ESP32-S3

This repository holds the Android app build for the Techstrivers ESP32-S3 robotic car. Android source code is stored in a zipped UTF-8/Base64 bundle (`android_bundle.b64`); the Actions workflow extracts the source then compiles a debug APK with Gradle and Android SDK.

## Build

Open **Actions → Build AI Robotic Controller APK** and choose **Run workflow**, or change `android_bundle.b64` to trigger a build. Download the `AI-Robotic-Controller-Debug-APK` artifact when the build succeeds.

The API key for OpenAI must be configured on a separate backend. No API keys, passwords, private PCB data, or credentials belong in this repository. The firmware uses a protective motor lock for initial testing.

**Notice:** This is a development APK, not a tested production release. Verify motors and GPIO wiring on the physical robot before enabling movement.