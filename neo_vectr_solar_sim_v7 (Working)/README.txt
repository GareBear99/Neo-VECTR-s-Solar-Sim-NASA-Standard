Neo-VECTR's Solar Sim v7

Updated from the current offline Neo-VECTR Solar Sim branch.

What's improved in this pass
- Aim-target zoom is tighter: wheel zoom now biases toward the nearest valid target under the cursor before descending.
- Unified graph travel is clearer across Universe -> Milky Way -> Star System -> Planet Surface.
- Added an Accuracy / Sources panel so truth data and render abstraction are visibly separated in the UI.
- Solar-system bodies remain authored from static orbital/body fields in this offline package.
- Surface view remains synth-first and switches into GPS-style lat/lon guidance at close zoom.

Controls
- Wheel: aim-target zoom
- Drag: pan, or rotate globe in surface mode
- Click: select object
- Enter: descend
- Backspace: ascend
- 1 / 2 / 3 / 4: force Universe / Milky Way / Star System / Planet Surface
- F: focus selected
- [ and ]: time scale
- Space: pause

Accuracy policy in this build
- Physical/orbital fields are treated as truth inputs.
- Visual scale compression, glow, and synthetic body rendering are presentation only.
- Galaxy and Milky Way layers are curated/synthetic overview shells, not full live catalog ingestion.
- Earth is still the strongest near-surface implementation; Moon and Mars share the same local renderer path.

Package
- Open index.html in a browser.
