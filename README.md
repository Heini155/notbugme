# notbug.me

**No loops. Just noise.**
Real-time synthetic noise for sleep, relaxation, and focus.

---

## English

### What is notbug.me?
**notbug.me** is a minimalist web app for continuous noise. The sound is generated live in the browser (Web Audio API), so there are **no audio files, no loops, and no audible transitions**.

Good for:
- Falling asleep without mental chatter
- Calm background ambience
- Focus and deep work

### Features
- Brown / Pink / White noise
- Real-time synthesis (no loops)
- Gentle fade-in / fade-out
- Sleep timer (30 / 60 / 90 / 120 min)
- Volume control
- Language switch (Deutsch/English) with auto-detect from browser
- Dark, minimal UI
- Works on desktop and mobile
- No accounts, no tracking

### Tech
- Web Audio API
- AudioWorklet (with ScriptProcessor fallback)
- Noise is generated sample-by-sample
- No external libraries
- Single-file `index.html`

> Why no loops?
> Looped audio often creates audible seams.
> notbug.me generates noise continuously, so there is no loop and no loop transition.

---

## Deutsch

### Was ist notbug.me?
**notbug.me** ist eine minimalistische Web-App fuer kontinuierliches Rauschen.
Das Rauschen wird live im Browser erzeugt (Web Audio API) - es gibt **keine Audiodateien, keine Loops und keine hoerbaren Uebergaenge**.

Ideal fuer:
- Einschlafen ohne Gedankenkarussell
- Ruhige Hintergrundgeraesche
- Fokus und Deep Work

### Features
- Brown / Pink / White Noise
- Echtzeit-Synthese (keine Loops)
- Sanftes Fade-in / Fade-out
- Sleep-Timer (30 / 60 / 90 / 120 min)
- Lautstaerke-Regler
- Sprachumschaltung (Deutsch/English) mit Auto-Erkennung
- Dark UI, minimalistisch
- Funktioniert auf Desktop und Mobile
- Keine Accounts, kein Tracking

### Technik
- Web Audio API
- AudioWorklet (mit Fallback auf ScriptProcessor)
- Noise wird Sample fuer Sample berechnet
- Keine externen Libraries
- Single-File `index.html`

> Warum keine Loops?
> Geloopte Audiodateien erzeugen oft hoerbare Uebergaenge.
> notbug.me berechnet das Rauschen kontinuierlich - es gibt keinen Loop, also auch keinen Loop-Uebergang.

---

### Lokal starten
```bash
git clone https://github.com/Heini155/notbugme.git
cd notbugme
python -m http.server 8080
```
Open http://localhost:8080 in your browser.
