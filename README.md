<div align="center">

# ✈️ FSCopilot

### Your hands-free, voice-controlled First Officer for Microsoft Flight Simulator

![Version](https://img.shields.io/badge/version-0.0.9-5c3fa1)
![Platform](https://img.shields.io/badge/platform-Windows%20x64-0078D6)
![Runs](https://img.shields.io/badge/100%25-Local%20%26%20Offline-2ecc71)
![License](https://img.shields.io/badge/license-Proprietary-626891)

**[⬇️ Download the latest release](https://github.com/DevDokus/FSCopilot/releases)**

</div>

> [!IMPORTANT]
> **FSCopilot is in early development (v0.0.9).** Some features may be incomplete, not work fully yet, or change significantly between releases. You're flying an early build — expect rapid changes, and thanks for being part of it! ✈️

---

## What is FSCopilot?

FSCopilot is a desktop companion app that turns your voice into cockpit actions inside **Microsoft Flight Simulator**. Instead of reaching for the mouse to find a switch mid-approach, you simply *talk to your copilot* — naturally, the way you would to a real first officer:

> *"Copilot, gear down."*
> *"Can you bring the flaps up, please."*
> *"Set the parking brake."*

Copilot hears you, understands what you meant, and performs the action in the sim — then gives you a short spoken confirmation so you can keep your eyes outside and your hands on the yoke.

---

## ✨ Key Features

- 🎙️ **Natural voice control** — speak conversationally; no rigid command syntax to memorize.
- 🧠 **Built-in AI brain** — a local language model interprets your *intent*, not just keywords.
- 🛩️ **Live aircraft dashboard** — real-time airspeed, altitude, heading, vertical speed, and more.
- 🎛️ **Full autopilot control** — heading, altitude, vertical speed, LNAV/VNAV, localizer, approach, level change, speed, and autothrottle arm/speed hold, all by voice.
- 🔇 **Echo-free conversations** — the microphone automatically pauses for the exact length of Copilot's own spoken reply, so it can never hear (and act on) itself.
- 🔊 **Spoken confirmations** — every action is read back so you always know it was heard.
- ⚙️ **Customizable settings** — adjust Copilot's volume, switch between voice-activation and push-to-talk, and configure regional transition altitudes to match where you fly.
- 🔒 **100% local & private** — no internet, no telemetry, no data collection. Ever.
- 🚀 **Auto-updating** — new versions install themselves seamlessly in the background.
- 🪟 **One-click installer** — a single Windows setup file; no dependencies to hunt down.

---

## ⬇️ Download & Installation

1. Head to the **[Releases page](https://github.com/DevDokus/FSCopilot/releases)**.
2. Download the latest **`FSCopilot-Setup-x.x.x.exe`** installer.
3. Run it. The installer sets up a Start Menu and desktop shortcut automatically.
4. Launch **FSCopilot**, start Microsoft Flight Simulator, and you're ready to fly.

> 💡 From here on, FSCopilot keeps itself up to date — when a new version is released, it downloads and installs in the background with a visible progress indicator. You'll always be on the latest build without lifting a finger.

**No additional software, runtimes, or models need to be installed separately** — everything Copilot needs is bundled inside the app.

---

## 🎧 How To Use It

1. **Start FSCopilot** and **Microsoft Flight Simulator**. The dashboard shows a green **Online** indicator once it's linked to the sim.
2. **Just talk.** Copilot is always listening in the background, but it only acts when you include an *activation phrase* so it won't react to ATC chatter or cabin conversation.
3. Activation phrases are intentionally natural — things like **"copilot"**, **"computer"**, **"can you…"**, **"please…"**, or **"set…"**. So all of these work:
   - *"Copilot, gear up."*
   - *"Can you lower the flaps?"*
   - *"Please set the parking brake."*

### Currently supported commands

| Command | Example phrasings |
|---|---|
| **Gear Down** | "gear down", "lower the gear", "wheels down" |
| **Gear Up** | "gear up", "retract the gear", "wheels up" |
| **Flaps Down** | "flaps down", "deploy flaps", "lower the flaps" |
| **Flaps Up** | "flaps up", "retract flaps", "raise the flaps" |
| **Parking Brake Set / Release** | "set parking brake", "apply the brakes", "release parking brake", "release the brakes" |
| **Set Heading** | "set heading 251", "turn heading 030", "fly heading 180" |
| **Engage Heading Hold** | "engage heading hold", "hold heading", "activate heading hold" |
| **Autopilot On / Off** | "autopilot on", "engage autopilot", "autopilot off", "disengage autopilot" |
| **Set Altitude** | "set altitude 210", "climb and maintain flight level 350", "set altitude five thousand" |
| **Engage Altitude Hold** | "engage altitude hold", "hold altitude", "capture the altitude" |
| **Set Vertical Speed** | "set vertical speed 1500", "vertical speed minus 1000", "descend at vertical speed 800" |
| **Engage Vertical Speed Mode** | "engage vertical speed", "vertical speed mode", "hold vertical speed" |
| **Lateral Navigation (LNAV)** | "engage LNAV", "activate lateral navigation", "follow the flight plan" |
| **Vertical Navigation (VNAV)** | "engage VNAV", "activate vertical nav", "vnav mode" |
| **Localizer (LOC)** | "engage the localizer", "capture the localizer", "arm the localizer" |
| **Approach (APP)** | "arm approach", "engage approach mode", "activate approach" |
| **Level Change (FLC)** | "engage level change", "activate level change", "flight level change mode" |
| **Set Speed** | "set speed 250", "select airspeed two five zero", "set the airspeed to 280" |
| **Arm / Disarm Autothrottle** | "arm the autothrottle", "engage the autothrottle", "disarm the autothrottle", "turn off the autothrottle" |
| **Engage Speed Hold** | "speed hold", "engage speed mode", "activate speed hold" (arms the autothrottle first if it isn't already) |

Each command understands many natural variations — the examples above are just a taste. The in-app **Commands** tab lists every phrase for each action, and the command set is actively growing release over release.

---

## 📊 The Live Aircraft Dashboard

The **Copilot** tab is a real-time glass panel fed directly by the simulator, refreshing several times a second:

- **Aircraft identity** — the current airframe's name and type, with a live connection indicator.
- **Primary instruments** — airspeed, altitude, heading, and vertical speed (with a climb/descent trend indicator).
- **True ground distance** — the altitude tile shows your real height above the terrain below you, accurate no matter how the altimeter is set.
- **System states** — landing gear, landing lights, parking brake, autopilot, and flaps.
- **Altimeter setting** — shown in both **inHg** and **hPa**, so it reads correctly no matter which region's procedures you fly.
- **Altimeter transition reminder** — triggers "SET STD" or "SET local pressure" alarms based on flight altitude and your region's configured transition altitude (see "Settings & Customization" below).
- **Speed limit warning** — displays custom visual and vocal alerts for exceeding 250 kts below 10,000 ft.
- **Landing lights reminder** — warns when landing lights are off below 10,000 ft or still active above 10,000 ft.
- **Autopilot Configuration panel** — every selector and mode (HDG, LNAV, VNAV, FLC, ALT, V/S, LOC, APP, SPD, autothrottle) lit up live when it's engaged, with the selected target values shown alongside.
- **Weather, Airport & Runway panel** — live wind, temperature, QNH and visibility; the head/crosswind component for a landing on your current heading; the nearest airport's ICAO code, elevation, distance and bearing; and your tuned COM/NAV radios and ILS details.

This gives you an at-a-glance overview of your aircraft without digging through cockpit menus — and it lays the groundwork for smarter, aircraft-aware commands in future updates.

---

## ⚙️ Settings & Customization

A dedicated **Settings** tab lets you tailor Copilot to how you fly, with every choice saved automatically on your PC:

- **Copilot Volume** — a slider for the voice and interface sound volume, applied live as you drag.
- **Listening Mode** — stick with continuous voice activation, or switch to **push-to-talk** and bind any key: press once to arm a single command, no wake word needed.
- **Remember App Position** — reopens the window at the size, position, and monitor you last used.
- **Transition Altitude Zones** — the altitude where you switch between local pressure and standard (1013 hPa / 29.92 inHg) varies by region. Configure it per zone with simple sliders (1,000 ft steps) — Default (Europe & anywhere unrecognized), North America, and Japan ship as examples, each independently adjustable to match real-world or custom procedures.

---

## ⚙️ How It Works (Under the Hood)

FSCopilot is a self-contained pipeline that takes raw microphone audio and turns it into a precise simulator action — all locally. At a high level, a spoken command travels through several stages:

1. **🎙️ Audio capture** — your voice is captured at the system level through an embedded, high-performance audio engine and normalized for speech processing. No external audio tools or driver setup required.

2. **🗣️ Speech detection** — rather than naively reacting to volume, a dedicated voice-activity model distinguishes genuine speech from background engine and cabin noise, so Copilot knows exactly when you start and stop talking.

3. **🔑 Activation gating** — before anything is interpreted, the sentence has to contain one of a broad, deliberately natural set of activation phrases. If none are present, the input is dropped immediately and never reaches the AI — so idle conversation, ATC, and cabin chatter never trigger an action.

4. **📝 Speech-to-text** — your words are transcribed by a built-in speech-recognition model that runs as a persistent, always-warm background service. Keeping it loaded between commands (instead of spinning it up each time) is a big part of why responses feel near-instant rather than laggy.

5. **🧠 Intent interpretation** — the transcribed text is handed to a compact, locally-run language model that works out what you actually *meant* and maps it onto one of your real, configured commands. This is where most of Copilot's engineering lives: the model's output is tightly constrained so it can only ever return a genuine command (or "unknown"), and additional validation layers independently sanity-check the result — for instance, catching cases where a control might otherwise be moved in the opposite direction to what you asked, or where two similarly-worded commands (like the autothrottle and the autopilot) could be confused for one another. Anything the system isn't confident enough about is quietly ignored rather than risking the wrong input.

6. **🎮 Execution** — the confirmed command is sent to Microsoft Flight Simulator through its **official SimConnect interface** — the same channel professional add-ons use. It sets the native simulator variable directly, exactly as if you'd moved the control yourself, so each aircraft's own systems and operating limits still apply.

7. **🔊 Confirmation** — a short spoken cue plays so you know the action was heard and carried out, without ever needing to glance away from the windscreen. The microphone is automatically paused for exactly as long as that reply takes to play, measured from the actual audio clip rather than guessed — so Copilot's own voice can never be picked back up and misread as your next command.

Alongside this command pipeline, FSCopilot keeps a separate, always-on link to the simulator that feeds the **live aircraft dashboard** and will power increasingly aircraft-aware behavior over time. Both connections re-establish themselves automatically if the simulator restarts or a flight is reloaded, so you rarely have to think about them.

### Technology at a glance

FSCopilot is an **Electron**-based Windows application that bundles a **local large language model** for reasoning, an **on-device speech-recognition engine** for transcription, a **neural voice-activity detector**, and a native **SimConnect** bridge to the simulator. The models are quantized and tuned to run efficiently on everyday gaming hardware, entirely offline.

> ℹ️ *FSCopilot is in active early development. The finer details of our prompt design, model tuning, reliability safeguards, and command-matching logic are part of what makes Copilot dependable — so while this overview explains the architecture, some of the secret sauce stays in the cockpit.* 😉

---

## 🔒 Privacy & Offline Guarantee

**FSCopilot processes everything locally on your machine.**

- ✅ The **only** program that ever touches the internet is the flight simulator itself (for its own normal operation). Apart from FSCopilot's built-in auto-updater checking for new releases, **none of Copilot's components — the language model, the speech engine, the voice detector, or any other process — can or do reach the internet.**
- ✅ **No user data is ever collected, transmitted, or stored.** Your voice, your transcripts, your prompts, and your flight data never leave your computer. There are no analytics, no tracking, and no cloud services.
- ✅ Audio is processed in-the-moment and discarded — it is not logged or retained.
- ✅ Every feature is fully self-contained and used strictly to power the application's core functionality.

In short: what happens in your cockpit stays in your cockpit.

---

## 💻 System Requirements

- **OS:** Windows 10 / 11 (64-bit)
- **Simulator:** Microsoft Flight Simulator, connected via SimConnect
- **Microphone:** any working input device
- **Hardware:** a typical flight-sim-capable PC; the AI runs comfortably alongside the simulator on everyday gaming hardware

---

## ⚠️ Disclaimer

FSCopilot is an independent, fan-made tool and is **not affiliated with, endorsed by, or associated with Microsoft, Asobo Studio, or any aircraft manufacturer.** It sends the same control inputs you could send yourself, so it remains bound by each aircraft's own flight model and operating limits. Always fly responsibly and treat Copilot as an assistant, not a replacement for pilot judgment.

---

**Made with ❤️ for the flight sim community by [DevDokus](https://github.com/DevDokus)**

**[⬇️ Get the latest version](https://github.com/DevDokus/FSCopilot/releases)**

---

## 📜 Full Changelog

<details>
<summary>Click to expand full history</summary>

### v0.0.9
- **Settings Page:** New tab for Copilot volume, push-to-talk binding, remember-window-position, and per-region transition altitudes — all saved to disk.
- **Push-to-Talk:** Optional alternative to continuous listening; press a bound key once to arm a single command, no wake word required.
- **Altitude & Vertical Speed by Voice:** Set a target altitude or vertical speed, or engage their hold modes, by voice.
- **More Autopilot Voice Commands:** LNAV, VNAV, Localizer, Approach, Level Change, and Speed Set.
- **Autothrottle Arm & Speed Hold:** Arm/disarm the autothrottle and engage speed-hold mode by voice; speed hold auto-arms the autothrottle first if needed.
- **More Reliable LNAV:** Engaging LNAV now primes heading mode first, matching a confirmed default-737 engagement quirk.
- **Accurate Ground Distance:** The altitude tile's "GND" reading now shows true height above terrain, independent of the altimeter setting, instead of raw terrain elevation.
- **Configurable Transition Altitudes:** Move the hardcoded region values into Settings, with adjustable sliders per zone.
- **Echo-Loop Prevention:** The microphone now pauses for the exact measured duration of Copilot's own spoken reply, so it can't hear and misinterpret itself.
- **Sharper Command Recognition:** Hardened the AI against confusing similarly-worded commands (notably autothrottle vs. autopilot), including a safety net that blocks a misrouted command from acting on the wrong system.
- **Autopilot Configuration Panel:** Live state of every autopilot selector and mode at a glance.
- **Weather, Airport & Runway Panel:** Live weather, landing wind components, nearest airport, and tuned radios/ILS.
- **Altitude & Heading Reference Cues:** Visual climb/descend and turn-to-heading reminders when a new target is selected.

### v0.0.8
- **Voice-Activated Standby:** Copilot sits quietly in "Standby" and only listens when it hears your voice.
- **Improved PC Performance:** Reduced idle background processing.
- **Parking Brake:** Set & Release functionality implemented.
- **Set Heading:** Dial in any heading via voice (e.g., "set heading 251").
- **Heading Hold:** Engage heading hold via voice.
- **Autopilot On/Off:** Voice control for autopilot with secure activation.
- **Altimeter Reminder:** Alerts for Standard/Local pressure settings based on altitude/region.
- **Speed Limit:** Warning for overspeed (>250 kts) below 10,000 ft.
- **Landing Lights:** Reminder for lights off/on based on 10,000 ft threshold.
- **Interface Polish:** Adjustable sound volume and faster status readiness.

### v0.0.7
- **Live Aircraft Dashboard:** Real-time data from the sim.
- **Simulator Data Fixes:** Modernized data requests and variable alignment.
- **Stability:** Fixed shutdown crashes and improved trend arrow smoothness.
- **Info Refresh:** Updated in-app documentation.
- **Speed-Up:** Faster transcription by keeping the engine loaded.
- **Logo Sound Fix:** Consistent sound playback.
- **Refactor:** Modularized codebase.
- **Build:** Leaner installer sizes.

### v0.0.6
- **Voice Commands:** Improved intent recognition and direction correction.
- **Speech Recognition:** Upgraded model and vocabulary priming.
- **Faster Reaction:** Dedicated VAD for better speech/noise detection and faster cutoff.
- **Security:** Sandboxed main window.
- **Cleanup:** Leaner builds and startup reliability fixes.

### v0.0.5
- **MSFS24 Connectivity:** Initial integration for gear and flaps.
- **UI/UX:** New Info hub, Commands view, and details modals.

### v0.0.4
- **AI Hardening:** Improved conversational grounding and directional logic.
- **UI:** Persistent response bar, dynamic versioning.

### v0.0.3
- **Voice Interaction:** Smart VAD and fluid sentence recognition.
- **AI Engine:** Contextual hints and JSON output hardening.
- **Stability:** Binary path fixes and artifact filtering.
- **UI:** Standby state and low-latency IPC.

### v0.0.2
- **Auto-Updater:** Seamless background updates with progress indicators.
- **Fixes:** Artifact standardization and ESM/CommonJS compatibility.

### v0.0.1
- **Launch:** Initial production framework and core AI integration.
</details>

