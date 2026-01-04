# notbug.me

**No loops. Just noise.**  
Synthetisches Rauschen in Echtzeit – für Schlaf, Entspannung und Fokus.

---

## 🇩🇪 Deutsch

### Was ist notbug.me?
**notbug.me** ist eine minimalistische Web-App für Einschlaf- und Konzentrationssounds.  
Das Rauschen wird **live im Browser erzeugt** (Web Audio API) – es gibt **keine Audiodateien, keine Loops und keine hörbaren Übergänge**.

Ideal für:
- Einschlafen ohne Gedankenkarussell
- Ruhige Hintergrundgeräusche
- Fokus & Deep Work

---

### Features
- 🎧 **Brown / Pink / White Noise**
- 🔁 **Keine Loops** (echte Echtzeit-Synthese)
- 🌊 Sanftes **Fade-in / Fade-out**
- ⏲️ **Sleep-Timer** (30 / 60 / 90 / 120 min)
- 🌑 Dark-UI, minimalistisch
- 📱 Funktioniert auf Desktop & Mobile
- 🧠 Keine Accounts, kein Tracking, keine Daten

---

### Technik
- Web Audio API
- **AudioWorklet** (mit Fallback auf ScriptProcessor)
- Noise wird **Sample für Sample berechnet**
- Keine externen Libraries
- Single-File `index.html`

> Warum keine Loops?  
> Geloopte Audiodateien erzeugen oft hörbare Übergänge.  
> notbug.me berechnet das Rauschen kontinuierlich – es gibt keinen Loop, also auch keinen Übergang.

---

### Lokal starten
```bash
git clone https://github.com/Heini155/notbugme.git
cd notbugme
python -m http.server 8080
