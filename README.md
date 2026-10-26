# ⚓ EDITH — Straw Hat AI Assistant

**Your First Mate. Your shadow. Your blade.**

EDITH is a fully local-capable Android AI assistant with One Piece soul and Madara-level arrogance.

## Features

- 🔥 Always-running foreground service (survives reboot)
- 🎤 "Hey EDITH" wake word
- 🗣️ Speech-to-Text + deep TTS voice
- 🧠 Offline rules + Groq / OpenAI online brain
- ♿ Full Accessibility control (tap, swipe, type, click)
- 🏴‍☠️ One Piece comic UI (gold, red, ocean, speech bubbles)
- 🎭 Personality modes: Normal / FIRE (Ace) / CONQUEROR (Madara)

## How to Build the APK

1. **Install Android Studio** (Hedgehog or newer recommended)
2. Open the `EDITH` folder as a project
3. Let Gradle sync
4. Open `app/src/main/java/com/edith/assistant/llm/LLMManager.kt`
5. Replace `YOUR_GROQ_API_KEY_HERE` with a free key from https://console.groq.com
6. Connect your phone or use emulator (API 26+)
7. Click **Run** ▶ or Build → Build Bundle(s) / APK(s) → Build APK(s)

The APK will appear in:
`app/build/outputs/apk/debug/app-debug.apk`

## First Launch Checklist

1. Grant **Microphone** permission
2. Tap **Start Brain** (starts the foreground service)
3. Tap **Unlock Power** → find EDITH → Enable Accessibility Service
4. (Optional) Disable battery optimization for EDITH
5. Say **"Hey EDITH"** or type a command

## Personality Commands

- "Switch to fire mode"
- "Activate conqueror mode"
- "My name is [Name]"
- "Who are you?"

## Notes

- Wake word currently uses Android's SpeechRecognizer (works, but battery hungry). For production, integrate Picovoice Porcupine.
- Accessibility is the real power. Without it, EDITH cannot control the screen.
- All online LLM calls go through Groq (very fast + free tier).

---

*"I am EDITH. I answer only to you."*
