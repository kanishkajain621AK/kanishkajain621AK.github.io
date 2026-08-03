# Screenshots — what to capture, what to redact

Every image slot already has a placeholder file in place, so the site looks right immediately.
**Replace each placeholder with a real screenshot using the exact same filename and path.** Nothing in
`index.html` needs editing.

Capture at **1600×1000 or wider**, save as PNG. Wider is fine — the layout crops to 16:10 in the grid and
shows the full image in the lightbox.

---

## Redact before you upload — read this first

You are publishing screenshots of a live business's admin systems on the open internet. Anything visible in
a screenshot is public forever, including in Google's image index.

**Always remove:**

| What | Where it hides |
|---|---|
| Customer names, phone numbers, email addresses, delivery addresses | Reviews moderation, loyalty accounts, order lists, courier dashboards |
| Order IDs and transaction references | Anywhere an order appears — these are often guessable/enumerable |
| API keys, tokens, account IDs, connector credentials | Metrixcia connector screens, integration settings |
| Internal URLs, staging hostnames, IP addresses | Browser address bar — crop it out or use a clean window |
| Employee names and internal usernames | Admin headers, "last edited by", audit trails |
| Supplier and vendor names, cost prices, margins | Product admin, purchase data |
| Anything under NDA with a client (Pujaghar, Shapify, Cambik work) | Get written permission before publishing client admin screens at all |

**How to redact properly:** draw solid filled rectangles over the data. Do **not** blur and do **not** pixelate —
both are reversible with enough effort, and blurred text is often recoverable. Solid black or solid grey boxes only.

**Substitute rather than redact where you can.** A reviews moderation queue full of black boxes looks worse than
one showing three plausible fake reviews from "Test Customer". If you can populate a staging store with dummy
data and screenshot that instead, the result is both safer and better-looking.

**Before publishing the GMV and SaaS-cost figures, get your employer's sign-off in writing.**
₹5 crore monthly GMV is Divine Hindu's commercial metric, not yours, and it's currently printed in large type
on the front page. Most founders are happy to have it public; some are emphatically not, and it's much easier
to ask first than to take it down after a competitor sees it. If the answer is no, the fix is small — say
"eight-figure annual GMV" instead, which is nearly as strong and reveals nothing specific.

---

## The shot list

### `images/divine-hindu/`
| File | What to capture |
|---|---|
| `01-home.png` | Storefront home page — hero, mega menu open if possible, collection rails |
| `02-pdp.png` | A strong product page — gallery, variants, trust badges, reviews section visible |
| `03-cart-upsell.png` | Cart drawer open with upsells showing |
| `04-combo-builder.png` | Build Your Own Combo mid-flow, with the tiered discount visible |
| `05-lighthouse.png` | **The single most valuable screenshot on the site.** Run Lighthouse mobile in Chrome DevTools on a product page, capture the score wheel with performance 90+. Include the URL so it's verifiable. |

### `images/reviews-loyalty/`
| File | What to capture |
|---|---|
| `01-reviews-widget.png` | Storefront review widget with media reviews visible |
| `02-reviews-admin.png` | Your moderation queue — **redact customer names/emails or use dummy data** |
| `03-loyalty-admin.png` | Loyalty rules, tiers and thresholds config screen |
| `04-loyalty-widget.png` | Customer-facing loyalty panel — use a test account, not a real customer |

### `images/ai-engine/`
| File | What to capture |
|---|---|
| `01-astrologer-dashboard.png` | The roster view showing many agents at once — the "30+" claim made visible |
| `02-agent-config.png` | One agent's configuration: persona, service, doctrinal constraints |
| `03-report-sample.png` | A few pages of a generated report side by side, ideally showing the page count. **Use your own birth details or dummy data, never a customer's.** |
| `04-order-flow.png` | Pipeline/queue status view showing orders moving through stages |

### `images/metrixcia/`
| File | What to capture |
|---|---|
| `01-dashboard.png` | The cross-channel dashboard — blended spend, ROAS, CAC. **Redact absolute spend figures if your employer prefers; the layout is what sells it.** |
| `02-connectors.png` | Connector list showing multiple sources and their token status. **Redact account IDs.** |
| `03-report-view.png` | A computed report or export view |

### `images/courier/`
| File | What to capture |
|---|---|
| `01-allocation-dashboard.png` | Carrier scores per area — the ranking logic made visible |
| `02-pincode-map.png` | Pincode serviceability/performance view |
| `03-rto-trend.png` | The RTO trend line falling after rollout. **Crop or hide the y-axis values** — you've chosen not to publish absolute rates, and the shape of the curve persuades without them. If in doubt, delete this slot. |

### `images/public-app/`
| File | What to capture |
|---|---|
| `01-app-admin.png` | The embedded Polaris admin of the public app |

### `images/theme/`
| File | What to capture |
|---|---|
| `01-theme-home.png` | Theme demo home page |
| `02-3d-showcase.png` | The 3D product showcase mid-rotation |
| `03-before-after.png` | The before/after slider mid-drag |

### `images/pujaghar/`
| File | What to capture |
|---|---|
| `01-home.png` | Home page |
| `02-combo.png` | Combo builder with stacked discounts visible |

### `images/shapify/`
| File | What to capture |
|---|---|
| `01-home.png` | Home page |
| `02-pdp.png` | Video-led product page |

---

## Priority order

If you only have an hour, do these six and publish — the rest can follow:

1. `divine-hindu/05-lighthouse.png` — proves the performance claim
2. `courier/03-rto-trend.png` — proves the logistics result (axis values optional)
3. `divine-hindu/01-home.png` — proves the storefront is real and looks good
4. `ai-engine/01-astrologer-dashboard.png` — proves the "30+ agents" claim
5. `divine-hindu/03-cart-upsell.png` — proves custom cart work
6. `metrixcia/01-dashboard.png` — proves the data platform exists

A portfolio with six real screenshots and twenty-one placeholders is worse than one with six real screenshots
and the rest of the slots deleted. If you're not going to fill a slot soon, delete that `<figure class="shot">`
block from `index.html` rather than shipping a placeholder that says "REPLACE THIS FILE".
