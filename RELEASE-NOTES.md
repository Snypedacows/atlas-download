# A.T.L.A.S. Mac beta — release notes

## 1.0.0 (2026-11-17) — Apple TV remote build

New in this build:
- Apple TV remote support built on reverse-engineered MediaRemote + Companion Link
  protocols (the pyatv approach): Bonjour discovery, PIN-pairing design, keychain-stored
  credentials, encrypted session, and remote commands (play/pause, navigation, app launch,
  volume, power).
- Configurable sleep-video library: up to five saved YouTube links, each named, selectable
  by name or number (1–5), with delete and swap per slot. Stored alongside the paired
  credentials. Preserves the bedtime sleep-video behavior from the Surface.

Important limitations:
- **Unofficial.** The Apple TV link uses reverse-engineered protocols, not an Apple API.
  It can break on a tvOS update and would be rejected from the App Store. It ships here in
  the Developer-ID-style DMG only.
- **Live PIN pairing is not wired up yet in this build.** The app discovers and shows an
  Apple TV by name, but does not yet prompt for the 4-digit PIN or open the live encrypted
  session, so it will not actually drive a TV yet. The bedtime routine and sleep-video
  library are built and tested; the live remote link is still to come.
- The app is ad-hoc signed and not notarized. If macOS blocks the first open, right-click
  the app, choose Open, then Open again.

Download is gated by a code on the page (soft gate, no real authentication).
