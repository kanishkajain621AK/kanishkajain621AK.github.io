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
| API keys, tokens, account IDs, connector credentials | Integration and settings screens |
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

The Lighthouse slot was removed from `index.html` rather than shipped as a placeholder. If you ever run
Lighthouse mobile on a product page and get a 90+ performance score, capture the score wheel **with the URL
visible** and I'll put the figure back — it's the only hard evidence for the 60 → 90+ claim on that page.

### `images/reviews-app/`
All six slots are filled with real screenshots. `02-moderation.jpg` has the four customer email
addresses covered with solid boxes — if you ever re-shoot it, redact them again.

| File | What it shows |
|---|---|
| `01-storefront-widget.jpg` | The widget on a product page |
| `02-moderation.jpg` | Moderation queue (emails redacted) |
| `03-overview.jpg` | Overview dashboard |
| `04-bulk-upload.jpg` | Bulk import |
| `05-widget-designer.jpg` | Display rules + widget designer |
| `06-add-review.jpg` | Manual review entry |

### `images/divine-points/`
All six slots are filled with real screenshots. The browser chrome was cropped off `03` and `05` because it
exposed the production hostname — if you re-shoot either, crop it again.

| File | What it shows |
|---|---|
| `06-checkout-redeem.jpg` | Redemption inside GoKwik one-click checkout — **the distinctive one**, shown first in the grid |
| `01-admin.jpg` | Program Flow — ways to earn / burn, referral |
| `02-storefront-widget.jpg` | Storefront customiser with live widget preview |
| `03-product-cashback.jpg` | Per-product / per-collection cashback overrides (hostname cropped) |
| `04-whatsapp-triggers.jpg` | WhatsApp lifecycle triggers and template mapping |
| `05-reports.jpg` | Finance reports and exports (hostname cropped) |

On `06`, the live UPI payment QR is covered with a solid box and the browser tab bar is cropped. If you
re-shoot it, do both again — a UPI QR encodes a payable intent and shouldn't be published.

### `images/super-app/`
Phone screenshots are portrait, so they'd be badly cropped by the 16:10 grid. Each file here is a **composite**
— two or three phone screens laid out side by side on a warm neutral canvas at 1600×1000.

| File | What it shows |
|---|---|
| `01-home.jpg` | Home, home scrolled to Best Sellers, navigation drawer (account name and number covered) |
| `02-jyotish.jpg` | Jyotish tab and the astrologer roster with consultation wallet |
| `03-content.jpg` | CMS-driven Our Story page and the store locator |

If you re-shoot any of these, keep the composite approach and cover the account name and phone number in the
drawer again. Three further screens (the founder photos on Our Story, and the Moments of Devotion gallery)
were left out because they show identifiable people — add them only if everyone pictured is fine with it.

### `images/ai-engine/`
Three slots filled with real screenshots of the Divine Jyotish dashboard.

| File | What it shows |
|---|---|
| `01-agents.jpg` | The agent roster — traditions, specialisms, languages |
| `02-report-generator.jpg` | Kundli report generation and the delivery log — **the four report filenames are covered with solid boxes**; they contained customer names and share-link tokens, so redact again if re-shot |
| `03-knowledge-base.jpg` | The shared knowledge base every agent reads from |

Still worth capturing: **one agent's edit-and-train screen**, which would show the persona and doctrinal
constraints an individual agent runs under — the roster proves breadth, but not depth. And a couple of pages
of a generated report side by side, using your own birth details or dummy data, never a customer's.

The roster shows six agents; the write-up claims 30+. Scroll the page and take a taller screenshot, or crop
to a grid that clearly continues past the fold, so the number on the page and the number in the picture agree.

### `images/public-app/` — ReviewMaster

All six slots are filled with real screenshots of the ReviewMaster development store.

| File | What it shows |
|---|---|
| `01-app-admin.jpg` | Embedded dashboard (browser chrome cropped) |
| `02-moderation.jpg` | All reviews — **two reviewer email addresses covered with solid boxes**, redact again if re-shot |
| `03-incentives.jpg` | Incentive setup with the no-minimum-rating panel — the highest-value shot on the project |
| `04-import.jpg` | Import sources and the provenance rules |
| `05-widgets.jpg` | The nine widget layouts |
| `06-settings.jpg` | Moderation, media and display settings |

Two things to know before re-shooting. The screenshots come from a **development store**, so the reviews are
test data and the `dev` badge is visible — that's honest for an app in review, but swap in a real merchant
store once one is installed. And the Shopify sidebar shows **Judge.me installed alongside ReviewMaster**; it's
harmless, and arguably good framing given the write-up names Judge.me as a competitor, but crop it if you'd
rather not.

Still worth capturing: the buyer-facing form at `/r/:token` on a phone mid-submission with a photo attached,
and the widget rendering on a live product page. Those are the only two customer-facing surfaces the gallery
doesn't show.

### `images/theme/`
`01-theme-home.jpg` is a real screenshot of the demo store's Spotlight section (browser chrome cropped) and is
the image on the "Also shipped" card.

| File | Status |
|---|---|
| `01-theme-home.jpg` | Real — demo store Spotlight section |
| `02-3d-showcase.png` | Placeholder — the 3D product showcase mid-rotation |
| `03-before-after.png` | Placeholder — the before/after slider mid-drag |

Neither placeholder is referenced by `index.html`, so nothing is broken; they're only worth capturing if the
theme gets promoted to a full case study.

### `images/pujaghar/`
| File | What to capture |
|---|---|
| `01-home.png` | Home page |
| `02-combo.png` | Combo builder with stacked discounts visible |

### `images/shapify/`
`01-home.jpg` is a real screenshot of the Cult Essentials collection grid (browser chrome cropped) and is the
image on the "Also shipped" card. `02-pdp.png` is still a placeholder and is not referenced by `index.html`.

---

## Priority order

Most galleries are now filled with real screenshots. What's left, in order of what it would prove:

1. **A Lighthouse mobile report** on a Divine Hindu product page, score wheel plus URL — the only hard evidence
   for the 60 → 90+ claim. The slot is currently removed rather than empty
2. A taller `ai-engine/01-agents.jpg` — the roster currently shows six agents against a "30+" claim
3. The ReviewMaster buyer form at `/r/:token` on a phone, and the widget on a live product page

A placeholder that says "REPLACE THIS FILE" is worse than no image. If a slot isn't getting filled soon,
delete its `<figure class="shot">` block from `index.html` instead of shipping the placeholder.

**MARG and AdCompass were removed from the site.** Their write-ups and image folders are gone from
`index.html` and `images/`. If they come back, the shot lists were: MARG — allocation tester (chosen origin
plus every rejected origin with its reason), Integrations, Warehouses, all three with the production hostname
cropped out. AdCompass — dashboard, weekly ranked test plan, strategy teardown, attention heatmap.
