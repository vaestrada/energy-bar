# ⚡ Quantum Roadrunner Energy Bar

A live interactive energy bar for the **Quantum Roadrunner: The Tech Run** fun run opening program. The crowd generates electricity through their energy — shouting, cheering, and moving charges the battery. When it hits 100%, the run begins!

**Live demo:** [vaestrada.github.io/energy-bar](https://vaestrada.github.io/energy-bar/)

## How It Works

A vertical battery displayed on a projector/LED wall fills up based on crowd noise (via microphone) or manual host control. The bar rises and falls in real time, creating an interactive moment before the run starts.

- **Mic mode** — crowd noise charges the bar; silence drains it
- **Manual mode** — host controls the bar with keyboard shortcuts
- **Auto mode** — bar rises and falls on its own with natural variation

When the battery reaches 100%: celebration screen with confetti, 100 kWh stat (enough to fully charge a ZEEKR 7X), and "LET'S RUN!"

## Quick Start

1. Open `index.html` in Chrome (local file or hosted)
2. Click **⚡ ACTIVATE ⚡** (grants microphone permission)
3. Press **F** for fullscreen
4. Press **P** to open the control panel

That's it — no dependencies, no build step, no install.

## Host Keyboard Shortcuts

| Key | Action |
|-----|--------|
| **↑ / ↓** | Increase / decrease energy |
| **Space** | Quick boost (+10%) |
| **R** | Reset to 0% |
| **F** | Toggle fullscreen |
| **M** | Mute / unmute mic |
| **+/-** | Adjust mic sensitivity |
| **S** | Cycle rising sound (Off → Chimes → Melody → Pad) |
| **P** | Toggle control panel |
| **H** | Toggle help overlay |
| **C** | Force celebration (100%) |

## Control Panel (press P)

| Control | Options |
|---------|---------|
| **Mode** | Mic, Manual, Auto |
| **Sensitivity** | Slider (mic mode only) |
| **Drain** | How fast the bar drains (0–20) |
| **Auto Speed** | Speed of auto mode animation |
| **Rising sound** | Off, Chimes, Melody, Pad |
| **Celebration sound** | Off, Sparkle, Arpeggio, Fanfare |
| **Volume** | Master volume slider |

## Sound Options

### Rising (as bar climbs)
- **Off** — silent
- **Chimes** — bell ding at every 10% milestone
- **Melody** — ascending pentatonic scale notes at milestones
- **Pad** — warm ambient tone that swells with energy level

### Celebration (at 100%)
- **Off** — silent
- **Sparkle** — twinkly notes cascading down then up
- **Arpeggio** — happy ascending do-mi-sol notes
- **Fanfare** — bold ta-da-da-DAAAA victory pattern

## Event Setup Tips

- **Projector/LED wall:** Open in Chrome, press F for fullscreen
- **App mode (no browser chrome):** Run `google-chrome --app=https://vaestrada.github.io/energy-bar/`
- **PowerPoint integration:** Add the URL as a hyperlink on a slide
- **If mic is too sensitive:** Open control panel (P), lower the Sensitivity slider
- **If mic causes issues:** Switch to Manual mode, use ↑ and Space
- **Backup:** Keep the `index.html` file on the event laptop — works offline

## Tech Stack

- Single `index.html` file — zero dependencies
- Vanilla HTML + CSS + JS
- Web Audio API for microphone input and synthesized sounds
- CSS animations for glow, particles, and effects
- Canvas API for confetti

## Credits

Built for the **Quantum Roadrunner: The Tech Run** fun run event.
ZEEKR Philippines is a proud sponsor.
