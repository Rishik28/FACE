# FACE prototype

Open `index.html` in a modern browser. No installation or build step is required.

This vertical slice includes eye clicking, escalating upgrades, pupil automation, the second-eye Focus synergy, pooled Dander from eyebrows, second-eyebrow Expression, local saving, 50%-efficient offline production (capped at eight hours), and a responsive composite-software interface. Arcade feedback includes click debris, impact recoil, animated streak feedback, escalating number pops, purchase hits, and feature-unlock splashes, with reduced-motion support.

The prototype now uses the exported Identikit part library under `assets/parts`. Eye, pupil, eyebrow, eyelid, nose, and mouth assignments are saved per subject. Reconstitution unlocks after 2,500 run Impressions, resets the economy, rerolls every assigned part, and adds a permanent +25% global production multiplier per revision; subsequent requirements scale by ×4.

Eyebrow Dander production is represented by a timed photographic-fragment wiggle and falling Dander specks. The second eyebrow receives a stronger paired motion. Calibration speed affects the pulse frequency, capped to keep the effect readable.

The eyelid slice adds Ocular Fatigue, manual blinking, Silver Dander, Lash Density, and independent Blink Reflex automation. Manual eye clicks gradually fall to 35% efficiency until a blink clears fatigue. Use the on-face **BLINK** control or press `B`. Blinks use an eight-frame, non-looping forensic-composite GIF that is restarted for every manual or automatic blink.

The **CALIBRATION** console (also toggled with the backtick key) grants test resources, clears fatigue, readies prestige, and runs the simulation at ×1, ×5, or ×10 speed. These controls are intended for pacing work rather than the final player-facing build.

The nose slice unlocks for 120 Silver Dander. It begins with one nostril and independently produces Air and Soft Boogies. Airway Patency and Real Dripper upgrade those passive tracks separately; Coarse Follicles upgrades active pooled-Dander generation from **PULL HAIR** or the `N` key. The second nostril doubles steady Air and triggers a Deep Breath every six simulated seconds, while further Deep Breath upgrades add +25% Air per level.

Nasal production has distinct feedback: breathing motion for Air, falling drips for Soft Boogies, and a sharp pluck recoil with Dander debris for nose hairs. Calibration now grants Air and Boogies.

Configuration and reusable visual-effect helpers have moved into `js/config.js` and `js/effects.js`. They remain classic browser scripts so the prototype still runs directly from `index.html` without a local server.

The composite uses a fixed-proportion facial canvas so feature spacing remains coherent across viewport heights. Eye, eyelid, and nose actions are performed directly on their artwork; visible action buttons have been removed. Upgrade cards show continuous affordability fill and stronger hover, press, focus, and purchase-confirmation states.

Upgrade controls use persistent DOM nodes rather than rebuilding their markup every animation frame. Simulation remains frame-driven, while routine UI synchronization is capped at 10 Hz and purchases render immediately. Text and attributes are patched only when their values change, preserving hover/press state and reducing layout work. Touch controls use manipulation mode with browser tap highlighting disabled.

The mouth economy and sound remain reserved for later slices.
