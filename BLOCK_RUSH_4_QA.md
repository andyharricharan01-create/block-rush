# Block Rush 4.0 beta verification checklist

The branch `feature/block-rush-4` is development-only. Do not merge until all manual browser checks pass.

## Critical acceptance tests
- [ ] Desktop at 1366x768 and 970x906: board, 3-piece tray, score and controls fit without scrolling.
- [ ] Mobile at 375x667 and 390x844: board and pieces visible simultaneously; touch drag, tap placement and previews align.
- [ ] All six modes display coloured placed blocks after placement AND after reload.
- [ ] Classic: 8x8 gameplay, three-piece replenishment, line clears, scoring and high scores unchanged.
- [ ] Junior: easier shapes; no timer; no advertising or purchases.
- [ ] Arcade: pause/resume and 90-second countdown; moving away preserves remaining time.
- [ ] Daily: date-seeded challenge; no undo.
- [ ] Adventure: completing required lines shows success, advances exactly one mission; failing does not advance.
- [ ] Zen: untimed mode retains score and saved progress.
- [ ] In each mode, place a block, switch modes, return, reload; unfinished round is restored.
- [ ] Restart cancellation preserves existing round. Confirmed restart clears only selected mode round.
- [ ] Undo restores board, piece tray and score consistently.
- [ ] Reduced motion and sound toggles persist.
- [ ] High-score keys from versions 2 and 3 are preserved.
- [ ] Backup export and restore work correctly.
- [ ] Privacy and no-advertising promise remains accurate.

## Automated static checks completed
- Independent `solid-tile` element retained for coloured blocks
- New mode selectors present
- Mission-success dialog logic added
- Save key remains mode-specific
- Arcade timer restarts after restoration
- Classic best-score key unchanged
- Viewport-height layout CSS retained

Browser interaction tests have **not yet been completed**, so this beta must not be treated as a verified release.
