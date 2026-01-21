# Discipline Day Timer

A beautiful, feature-rich daily activity timer for managing your day with sequential focus blocks. Built as a single HTML file with no dependencies.

![Version](https://img.shields.io/badge/version-2.1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Features

- **Sequential Timer Blocks** - Create a schedule of timed activities that run in sequence
- **Visual Alerts** - Screen flash notifications when timers complete (configurable per timer)
- **Audio Alerts** - Customizable beep patterns with adjustable count, length, gap, and volume
- **Break Mode** - Timers starting with "Break" display a soothing green gradient background
- **Per-Timer Settings** - Each timer can have individual settings for:
  - Sound alerts (on/off)
  - Flash alerts (on/off)
  - Show seconds display (on/off)
- **Persistent Storage** - Your schedule and settings are saved to localStorage
- **Import/Export** - Save and load schedules as JSON
- **Responsive Design** - Works on desktop and mobile devices
- **Dark Theme** - Easy on the eyes with a beautiful gradient dark theme

## Usage

### Quick Start

1. Open `timer_revision_2_1_0.html` in any modern web browser
2. Click "Load Sample" to load a pre-built daily schedule, or
3. Add your own segments using the "Build Your Day" panel

### Controls

- **Start/Pause/Resume** - Single button that adapts to timer state
- **Previous/Next** - Navigate between timer segments (silent, no alerts)
- **Reset Day** - Stop the timer and return to the first segment

### Global Settings

- **Loop Schedule** - Automatically restart from the beginning when all timers complete
- **Auto-start Next** - Automatically begin the next timer when one completes

### Sound/Flash Settings

Expand the "Sound/Flash Settings" panel to configure:

- **Beeps/Flashes (count)** - Number of beeps/flashes when a timer completes (1-10)
- **Beep Length** - Duration of each beep in seconds (0.05-1.00)
- **Gap Between Beeps/Flashes** - Pause between each beep/flash (0.00-1.00)
- **Volume** - Audio volume level (0-1)

### Per-Timer Options

Each timer in your schedule can be configured individually:

| Option | Description |
|--------|-------------|
| Sound | Enable/disable audio beeps for this timer |
| Flash | Enable/disable screen flash for this timer |
| Show Seconds | Display full MM:SS or just minutes |

### JSON Format

Export and import schedules using this JSON format:

```json
[
  {
    "name": "Work Session",
    "seconds": 1500,
    "sound": true,
    "flash": true,
    "showSeconds": true
  },
  {
    "name": "Break",
    "seconds": 300,
    "sound": true,
    "flash": true,
    "showSeconds": false
  }
]
```

## Installation

No installation required! Simply:

1. Download `timer_revision_2_1_0.html`
2. Open in your web browser
3. Start timing!

Or host it on any web server or GitHub Pages.

## Browser Compatibility

Works in all modern browsers:
- Chrome (recommended)
- Firefox
- Safari
- Edge

Note: Audio requires user interaction on first use due to browser autoplay policies.

## Local Storage

The app stores the following in your browser's localStorage:

- `multiTimerSchedule_v3` - Your timer schedule
- `multiTimerSettings_v3` - Global settings (loop, auto-start, sound settings)

Clear your browser data to reset to defaults.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - Feel free to use, modify, and distribute.

## Changelog

### v2.1.0
- Added screen flash alerts with per-timer toggle
- Combined Start/Pause/Resume into single smart button
- Renamed "Stop/Reset" to "Reset Day"
- Updated time display to hide `:00` when seconds are disabled
- Compact schedule display with responsive single-line layout
- Added version footer with GitHub link
- Renamed settings section to "Sound/Flash Settings"

### v1.3.2
- Added collapsible sound settings panel
- Moved Sound and Show Seconds options to per-timer settings
- Added Previous/Next navigation buttons
- Green gradient background for Break timers
- Silent navigation (no alerts when using Previous/Next)

### v1.3.1
- Initial public release
- Sequential timer blocks
- Configurable audio alerts
- Import/Export JSON schedules
- Persistent localStorage settings

---

Made with ❤️ for productivity enthusiasts
Forked from https://github.com/jbaker-tech/Daily-Activity-Timer
