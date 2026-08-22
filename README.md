# MF Radio

MF Radio is a self-contained retro web jukebox for a collection of 102 MP3 tracks. Press play, then listen in shuffled order without repeats until the complete collection has played.

## Features

- 102-track shuffled playlist
- No repeats within a shuffle cycle
- Smooth transitions using two audio elements and the Web Audio API
- Animated record, tonearm, LED display and live 18-band frequency spectrum
- Play/pause, next-track and volume controls
- Keyboard shortcuts
- Responsive layout for desktop and mobile
- Bundled display and monospace fonts for consistent rendering across devices
- Screen wake lock while playing on supported mobile browsers
- Lock-screen and system media controls through the Media Session API
- Background track changes avoid throttled visual transition timers
- Reduced-motion support
- No external libraries, accounts or tracking

## Controls

| Action | Mouse / touch | Keyboard |
| --- | --- | --- |
| Start / resume | Red play button | Space or Right arrow when stopped |
| Pause | Red button | Space or Left arrow |
| Next track | Amber button | N or Right arrow while playing |
| Volume | Drag or scroll the knob | Up / Down arrows |

## Mobile playback

While music is playing, supported touch devices request a screen wake lock so the display does not dim automatically. If the screen is switched off deliberately or the browser moves to the background, playback continues through the regular media element and can be controlled through the operating system's media controls.

Screen wake lock requires HTTPS (or localhost) and can be declined by the browser, battery saver or low-power settings. A mobile operating system may still terminate any browser tab under memory or battery pressure; a website cannot override that system decision.

## Project structure

- `index.html` — complete interface, styling and player logic
- `assets/Motherfuckers_0.mp3` through `assets/Motherfuckers_101.mp3` — audio collection
- `assets/fonts/` — bundled Anton and Roboto Mono fonts with their OFL licenses
- `noise.html` — earlier standalone experiment retained separately

## Run locally

The audio files should be served over HTTP rather than opening `index.html` directly:

```powershell
python -m http.server 8080
```

Then open <http://localhost:8080/>.
