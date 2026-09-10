# ADX AI Assistant — Final Advanced Android Project

This is the **advanced Android Studio source project** for ADX AI Assistant.

## What is included

The app UI and project architecture cover the full ADX target roadmap inspired by the supplied Maya reference:
- AI chat + configurable AI provider
- Hindi/English voice input
- Voice assistant controls and wake/sleep settings
- Long-term local memory foundation
- User rules
- Teach/save routines (macros)
- Phone actions and intents
- Calls/SMS/contacts launch flows
- WhatsApp / WhatsApp Business launch flows
- Notifications permission + notification-listener entry point
- Screen sharing permission flow
- Camera capture flow
- Web research / coding / documents / markets / whiteboard module hub
- PC ↔ phone link foundation
- Smart-home connector foundation
- GitHub / Notion / Telegram connector settings
- Backup/export and restore foundation
- Background-work architecture hooks
- Advanced safety/permission settings
- 17-suite capability catalog and 150+ action roadmap UI
- GitHub Actions APK build workflow

## Important

Some capabilities require external services, Android special permissions, or third-party APIs.
The project **does not fake these as completed**. The app provides real Android entry points and configuration where practical, and clearly marks integrations that require setup.

For real AI answers, enter an API key for an OpenAI-compatible endpoint in Settings.
For production, do not ship a provider secret directly inside an APK; use a secure backend/token exchange.

## Open in Android Studio

1. Extract the ZIP.
2. Open the extracted `ADX_AI_Assistant_FINAL_ADVANCED` folder in Android Studio.
3. Let Gradle sync.
4. Connect an Android phone with Developer Options + USB debugging enabled, or start an emulator.
5. Press **Run**.
6. To make an APK: **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.

The project uses:
- Android Gradle Plugin 8.7.3
- Kotlin 2.0.21
- Gradle 8.10
- compileSdk 35
- minSdk 26
- targetSdk 35

## GitHub Actions

The included workflow installs Gradle 8.10 directly, so the repository does **not** depend on a missing `gradlew` wrapper JAR.

Push the complete project to GitHub, then:
**Actions → Build ADX Debug APK → Run workflow**

The generated debug APK is uploaded as a workflow artifact.

## Android permissions

The manifest declares only permissions needed by the included capabilities. Android may still require the user to grant runtime/special permissions manually.

## Production next steps

For a true production autonomous agent, connect:
- secure AI backend/provider
- speech-to-text + text-to-speech provider
- offline wake-word engine
- accessibility automation service with explicit user consent
- notification listener service
- MediaProjection/screen understanding
- camera vision model
- web research/search backend
- document generation/parsing backend
- market-data provider
- PC companion
- WhatsApp-compatible official integrations where permitted
- social-media APIs
- smart-home/Home Assistant/MQTT or vendor APIs
- secure authentication and encrypted token storage

The source is designed so those modules can be added without replacing the main ADX UI.
