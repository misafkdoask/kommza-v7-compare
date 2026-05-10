# Kommza V7 — design comparison set

**Live preview:** https://misafkdoask.github.io/kommza-v7-compare/

Internal artifact для выбора design-направления для Kommza V7. **Не для деплоя.**

## Что это

9 prototype-страниц с одним и тем же копи Kommza V6, упакованным в design-DNA популярных брендов из коллекции [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md). Coral `#F97316` сохранён везде как primary CTA. Меняется bg, типографика, радиусы, layout-rhythm, decoration.

| # | File | Direction |
|---|---|---|
| — | [`compare.html`](compare.html) | Index с превью всех 9 |
| 01 | [`01-mastercard.html`](01-mastercard.html) | Editorial cream + circular video portraits + ghost watermark + ink footer |
| 02 | [`02-airbnb.html`](02-airbnb.html) | White + pill search hero + soft photo cards |
| 03 | [`03-calcom.html`](03-calcom.html) | White + product UI mockup в hero + UI fragments в feature cards + dark navy footer |
| 04 | [`04-linear.html`](04-linear.html) | Pitch-black canvas + dashboard hero + radial coral glow + charcoal panels |
| 05 | [`05-notion.html`](05-notion.html) | Navy hero band + workspace mock + warm beige body + pastel feature cards |
| 06 | [`06-apple.html`](06-apple.html) | Edge-to-edge alternating tiles + SF Pro tight + cinematic video room mockup |
| 07 | [`07-vercel.html`](07-vercel.html) | Pure white + Geist-style tight tracking + shadow-as-border + JetBrains Mono captions |
| 08 | [`08-stripe.html`](08-stripe.html) | Radial gradient mesh hero + weight-300 elegance + tabular numbers + cream band |
| 09 | [`09-sanity.html`](09-sanity.html) | Pitch-black + Space Grotesk 112px + IBM Plex Mono uppercase eyebrows + tech-grid |

## Cross-model review

| Бренд | Codex | GPT-5.5 | DeepSeek | Self | Verdict |
|---|---|---|---|---|---|
| 01 Mastercard | средний | TOP — trust/warmth | **#1 obvious choice** (80% fit V6) | хорош | 🟢 финалист |
| 03 Cal.com | **#1 base** | **#1 category fit** | — | risk: scheduling-leak | 🟢 финалист |
| 05 Notion | TOP-3 SMB-friendly | TOP — "без IT-отдела" | TOP-3 для freelance | risk: Notion-clone | 🟢 финалист |
| 08 Stripe | TOP-3 premium | premium-fintech | weight-200 mobile fail | gradient mesh AI-tell | 🟡 спорно |
| 09 Sanity | слабый dev | слабый contrarian | TOP-3 для агентств | dev-tell для SMB | 🟡 спорно |
| 06 Apple | "музей" слабо | "не для меня" | — | Apple-ad-копия risk | 🟡 средне |
| 02 Airbnb | marketplace mismatch | search=маркетплейс | "Забронировать номер" | ♡=buy-pattern | 🔴 нет |
| 04 Linear | dev/infra-узкий | разрушает "просто" | dark+dev для SMB страшно | dev tell | 🔴 нет |
| 07 Vercel | dev/infra-узкий | mono+terminal=anti-сигнал | — | terminal=dev | 🔴 нет |

## Source spec

- [google-labs-code/design.md](https://github.com/google-labs-code/design.md) — Apache 2.0, формат
- [VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md) — MIT, 71 brand collection

## Локально

```bash
git clone https://github.com/misafkdoask/kommza-v7-compare.git
cd kommza-v7-compare
python3 -m http.server 9200
open http://localhost:9200/compare.html
```
