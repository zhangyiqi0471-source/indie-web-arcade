# itch.io Publishing & Monetization Checklist — Neon Void Survivor

## 1. One-Time Shell Creation (30 seconds on itch.io Dashboard)
> Note: itch.io blocks automated creation of brand-new project URLs to prevent spam. Once the blank shell `neon-survivor` exists, `butler` handles 100% of uploads and updates automatically!

1. Open: https://itch.io/game/new
2. **Title**: `Neon Void Survivor`
3. **Project URL**: `https://<your-itch-username>.itch.io/neon-survivor`
4. **Kind of project**: `HTML` (embeds `neon-survivor-html5-demo.zip` directly in browser!)
5. **Pricing**:
   - Choose **$0 or donate** at page level, THEN set **`neon-survivor-full-offline.zip` minimum price = `$9.99`**!
   - Result: Players play the HTML5 Demo in browser for free -> pay `$9.99` right below to unlock/download `neon-survivor-full-offline.zip`!
6. **Generative AI Disclosure (2026 Compliance)**:
   - Uses Generative AI Assets (Art/Audio/Text)? **No (Procedural / hand-crafted visuals; standard game code logic is exempt on itch.io)**
7. **Tags**: `roguelike, arcade, bullet-heaven, html5, cyberpunk, indie`
8. Upload Cover Image: Use `storefront/cover.svg` (or PNG export, 630x500).

## 2. Automated CLI Upload Commands (Handled by `gamepub deploy --targets itch`)
```bash
butler push dist/neon-survivor/itch/neon-survivor-html5-demo.zip <your-itch-username>/neon-survivor:html-demo --userversion 1.0.0
butler push dist/neon-survivor/itch/neon-survivor-full-offline.zip <your-itch-username>/neon-survivor:full-edition --userversion 1.0.0
```

## 3. Copy-Paste itch.io Store Description (Markdown)
```markdown
## Neon Void Survivor
**Dash, auto-fire plasma orbitals, and survive escalating cyber-swarms in 60 FPS HTML5 Canvas.**

Neon Void Survivor is a fast-paced cyber-arcade bullet-heaven roguelike built in pure HTML5 Canvas. Dodge geometry swarms, collect XP shards to evolve your plasma weapon, and push past Wave 3 in the Full Edition!

### What's in the Full Edition ($9.99)?
- Unlimited playtime & endless waves (no demo timer)
- Full offline standalone package (play anytime, anywhere)
- Supports independent micro-game development!
```
