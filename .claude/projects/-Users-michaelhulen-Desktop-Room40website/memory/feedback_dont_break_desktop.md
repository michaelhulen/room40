---
name: Don't break desktop when making mobile changes
description: User explicitly warned not to create problems on desktop version when optimizing for mobile
type: feedback
---

Don't mess up the desktop version when making mobile changes. Be careful and conservative.

**Why:** User doesn't want to have to fix regressions on desktop caused by mobile optimizations.

**How to apply:** When making responsive/mobile changes, never modify the original desktop image files or desktop CSS. Only add new mobile-specific assets and use `<picture>`/`srcset` so the browser picks the right one. Always keep the original files untouched.
