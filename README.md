# Workout — Block 3: The Long Ramp

Fresh PWA. Fresh repo. Your Blocks 1-2 history is baked in (31 sessions, junk sets filtered, OHP plates-per-side entries corrected to totals).

## Deploy (5 min)
1. GitHub → New repository → name it `workout-b3` → Public → Create.
2. On the empty repo page, "uploading an existing file" → drag ALL files in this folder (they're flat on purpose, no subfolders) → Commit.
3. Settings → Pages → Branch: `main`, `/ (root)` → Save. Wait ~1 min.
4. iPhone Safari → `https://YOUR-USERNAME.github.io/workout-b3/` → Share → Add to Home Screen.

Keep the old app installed until you're happy, then delete it. They don't share data and won't fight.

## What's different from Block 2's app
- One number to beat, huge, on every exercise, with last session's actual sets right under it
- Weight moves when SET 1 hits the top of the range at or under cap (no more all-3-sets-vs-RPE-cap deadlock)
- Session clock starts on your first logged set, not when the app breathes on a screen
- Week is derived from the calendar (block starts on your first finished session), no manual week button
- Week 4 is a mandatory deload: everything auto-drops 20%, cap 6
- Junk sets (1-2 reps at RPE ≤2) are ignored by the engine and called out at finish
- Core gate requires all 3 sets, not one token rep
- 3-days-in-a-row warning on the home screen
- Bodyweight is the hero stat (log daily-ish, sparkline included); tonnage is gone
- Career tab: lifetime PRs across all three blocks, rep PRs count via estimated 1RM
- Every exercise has a swap variant (DB/hotel fallbacks) with its own independent history, for the Chicago move
- Service worker is network-first: push an update to GitHub, force-close the app, reopen, you have it
- Import accepts old Block 1/2 backups too (dedupes against what's baked in)

## Backups
Career tab → EXPORT JSON BACKUP, weekly. The app nags when you're overdue. iPhone localStorage is a handshake deal with Apple.
