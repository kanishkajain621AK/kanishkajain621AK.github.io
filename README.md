# Portfolio — Kanishka Jain

Source for my engineering portfolio. **Live at [kanishkajain621ak.github.io](https://kanishkajain621ak.github.io)**

I'm a Shopify engineer in Gurgaon, India, and the sole engineer behind a D2C business trading at roughly
US$600K a month — an 800-SKU storefront hand-coded in Liquid, two custom Shopify applications that replaced
over US$1,000/month of third-party SaaS, a cross-platform app on the Play Store, and an AI platform running
30+ domain-tuned agents. Alongside it, a public multi-tenant Shopify app and a premium Online Store 2.0 theme,
both in review with Shopify.

The client work is proprietary, so the site presents each system as a case study — problem, constraints,
architecture, decisions, measured result — rather than as a repository. Every system is one I can demo live
on a call.

## What's in the portfolio

| System | What it is |
|---|---|
| 800-SKU D2C Shopify storefront | Divine Hindu — hand-coded Liquid theme, ~US$600K/month, Lighthouse 60 → 90+ |
| Product reviews app for the Shopify App Store | ReviewMaster — public multi-tenant SaaS, in review, Protected Customer Data Level 2 |
| In-house reviews & ratings system | Custom Shopify app — 10,065 reviews across 918 products, operated daily by non-technical staff |
| In-house loyalty program system | Points, cashback and redemption settled inside a third-party one-click checkout |
| Cross-platform mobile shopping app | React Native on the Play Store — commerce, on-device astrology, live consultations |
| AI report generation & delivery platform | 30+ domain-tuned agents turning storefront orders into delivered PDF reports |
| Premium Shopify theme for the Theme Store | Prominent — 97/100 performance, 100/100 accessibility, 121 KB total JS |
| Devotional-goods storefront | Pujaghar — combo builder, stacked discounts, flash-deal unlocks, certificate traceability |
| D2C apparel storefront | Shapify — video-led product pages, BOGO logic, prepaid incentives |

## Built with

No framework, no build step, no dependencies. One self-contained `index.html`: hand-written HTML and CSS,
CSS custom properties for theming, inline SVG for the architecture diagrams, and a small block of vanilla
JavaScript for the theme toggle, screenshot lightbox, scroll-reveal animations, category filtering, scrollspy
and the reading-progress bar. Every animation runs on transform and opacity only (compositor-friendly) and
the whole motion layer disables itself under `prefers-reduced-motion`. Responsive down to 390px, light and
dark modes, no external requests.

## Structure

| Path | What it is |
|---|---|
| `index.html` | The entire site |
| `images/` | Screenshots, one folder per project |
| `DEPLOY.md` | How this is deployed and updated |
| `SCREENSHOTS.md` | Shot list and redaction rules |

## Contact

[kanishkajain621@gmail.com](mailto:kanishkajain621@gmail.com) ·
[LinkedIn](https://www.linkedin.com/in/kanishka-jain-ak)
