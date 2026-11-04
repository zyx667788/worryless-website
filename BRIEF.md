# Website Draft Brief — Worryless Logistics (shared by all designers)

## Client
- Company: **Shenzhen Worryless International Logistics Co., Ltd.** (brand: WORRYLESS LOGISTICS, monogram "WL")
- Industry: international freight forwarding / cross-border logistics, based in Shenzhen, China. Target audience: overseas (mainly US) importers, e-commerce / Amazon sellers.
- Core services the client wants pushed (highest priority):
  1. **China to USA Air Freight DDP** (door-to-door, duties paid)
  2. **China to USA Sea Freight DDP**
- Reasonable secondary services (draft only, client will confirm): Amazon FBA shipping, customs clearance & last-mile delivery, warehousing.
- Contact (found online, NOT confirmed by client — keep but it's fine): email `jason@worryless.cn`; address: Room 201, Building E, Hourui No.3 Industrial Zone, No.2 Kaicheng Road, Hangcheng Sub-district, Bao'an District, Shenzhen, Guangdong, China. Phone / WhatsApp unknown → use `+86 XXX XXXX XXXX`.
- Existing site: https://www.worryless.cn/ ; reference site the client likes: https://forestleopard.com/

## Client's own words (from chat, translated)
- "I want a website. Design a set of images. International logistics industry."
- "Images are fairly simple — airplanes, cars/trucks, ships, that kind of thing. Just put the company logo and name on."
- "About 30–40 images. Pages don't need many images; except the homepage, everything else is small images. Homepage should have 3–4 big images."
- Banner size: **1920 × 750**.
- Deliverable now: **an HTML file** the client can open in a browser.

## Brand assets
- Logo: `assets/logo.jpg` (1280×1280, **white background, not transparent**). Black + metallic gold "WL" monogram with airplane and shipping container, wordmark "WORRYLESS LOGISTICS". Colors: near-black (#111) and gold gradient (~#8a6a1f → #d4af37 → #f3d98b).
  - Because the JPG has a white background, on dark surfaces place it inside a light container/chip, or crop with `object-fit`/`object-position` sensibly. Never stretch it.

## Photos (being generated concurrently — may not exist yet when you start)
Paths relative to `draft/`:
| File | Content | Ratio |
|---|---|---|
| `assets/images/hero-air.jpg` | cargo airplane being loaded / taking off, airport, dusk | 1920×750 |
| `assets/images/hero-sea.jpg` | container ship at sea, aerial | 1920×750 |
| `assets/images/hero-port.jpg` | container port with cranes, night/dusk | 1920×750 |
| `assets/images/svc-air.jpg` | air cargo pallets / plane hold | square |
| `assets/images/svc-sea.jpg` | stacked shipping containers | square |
| `assets/images/svc-fba.jpg` | modern warehouse with parcels / shelving | square |
| `assets/images/svc-delivery.jpg` | delivery truck on US highway | square |

Always give image containers a tasteful CSS gradient `background-color`/`background-image` fallback so the page still looks designed if a file is missing.

## Homepage sections required (from the client's site-building checklist)
1. Header / nav (Home, Services, About, Tracking, Contact) + "Get a Quote" CTA
2. Hero banner carousel, 3 slides, 1920×750 ratio on desktop (slides: brand/global, Air DDP, Sea DDP)
3. Hot services (4–8 cards; Air DDP and Sea DDP must be the most prominent)
4. Company advantages (why choose us)
5. Short company introduction (+ video placeholder or image)
6. Certificates area (placeholders — client will supply)
7. Application scenarios (e.g. e-commerce sellers, Amazon FBA, B2B wholesale, oversized cargo)
8. Contact info + quote form, footer

## Hard rules
- Single self-contained HTML file: inline `<style>` and `<script>`, vanilla JS, no frameworks, no CDN JS. Web fonts optional (provide good system fallbacks).
- All copy in **English**, professional freight-forwarder tone. No lorem ipsum.
- **Do not invent facts**: no made-up years in business, shipment counts, certificates, awards, client names or testimonials. Use clearly marked placeholders such as `XX+` or `[Certificate]`.
- Responsive: looks right at 1920, 1440, and 390 px wide. Mobile nav works.
- Accessible basics: semantic HTML, alt text, sufficient contrast, carousel has prev/next/dots and pauses on hover, respects `prefers-reduced-motion`.
- The page must not look like a generic AI template — make deliberate typographic and layout choices that fit your assigned direction.
