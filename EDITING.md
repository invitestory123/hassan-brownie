# Customer Editing Guide — wax-seal-royale (Hassan & Brownie)

This template is configured for **Hassan & Brownie — 1st Month Anniversary & 1st Kiss**, featuring an interactive wax-seal envelope overlay, opening video animation, swan background video, classical ambient music, countdown timer, romantic milestones, featured couple portrait with animated floating rose petals, and anniversary details.

---

## Normal Customer Changes

All routine customer edits are configured in:
→ `editable/wedding-data.js`

### Couple Information
Edit `couple` in `editable/wedding-data.js`:
- `groom`: "Hassan"
- `bride`: "Brownie"
- `title`: "1st Month Anniversary"
- `subtitle`: "1st Kiss"

### Date & Love Note
Edit `wedding` in `editable/wedding-data.js`:
- `dateLabel`: e.g. `"1st Month Anniversary"`
- `dateISO`: Event/anniversary ISO timestamp with timezone offset (`"2026-12-02T18:00:00+05:30"`). Drives live countdown timer and Google Calendar link.
- `invitationNote`: Main love note (`"thirty daays since that magi moment, and im still falling for you more and more  every single day"`)

### Milestone Timeline
Edit `schedule` array in `editable/wedding-data.js`:
- Five milestone rows with `title` and `time`.

### Media & Assets
Replace files directly in `editable/assets/` or update `media` in `wedding-data.js`:
- `photo`: Couple photo (`editable/assets/hassan-brownie.jpg`)
- `overlayImage`: Wax-seal envelope graphic (`editable/assets/ChatGPT Image Jun 23, 2026, 04_40_29 PM.png`)
- `sealVideo`: Wax-seal breaking/opening MP4 (`editable/assets/1782224012851.mp4`)
- `heroVideo`: Ambient background video (`editable/assets/Swans2.mov`)
- `audio`: Background soundtrack (`editable/assets/Einaudi_ Divenire (1) (1).mp3`)

---

## Rules for Future Agents

1. Make customer content edits in `editable/wedding-data.js` and replace media in `editable/assets/`.
2. Do not modify bundled Tilda core scripts in `js/` or styling in `css/`.
3. Keep ISO date strings with proper timezone offsets (e.g. `+05:30`).
4. Validate changes with `node --check editable/wedding-data.js`.
