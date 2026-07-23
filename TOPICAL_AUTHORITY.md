# Topical Authority — Florist.co.id

## Role and boundary

`Florist.co.id` is the direct-to-customer and organizational florist property for understanding, specifying, ordering, receiving, displaying, caring for, and responsibly disposing of floral products and event-floral work in Indonesia. Its primary readers are gift buyers, families, corporate buyers, wedding and event teams, hospitality/workplace teams, recipients, and florist practitioners who need reliable product and craft guidance.

The knowledge layer covers cut flowers, arrangement forms, floral design, occasions, order briefs, pricing structure, availability, freshness, delivery, care, safety, and material impacts. Existing product, service, checkout, and genuinely evidenced service-area routes retain transactional intent. Articles do not promise live stock, price, delivery time, nationwide coverage, plant safety, allergy absence, medical treatment, event performance, or firsthand project results.

`Floral.id` is a separate Syamsul-owned floral property and may independently cover the same flowers, products, craft, or queries. For portfolio context, `Florist.co.id` emphasizes buyer-to-recipient service and florist execution; `Floral.id` can retain its commerce, craft, and partner-network viewpoint. Cross-domain overlap is allowed. Cannibalization controls in this document apply only within `Florist.co.id`.

## Evidence audited

- Canonical decision: `cfpages-adminalampintar/Florist.co.id`, branch `main`. Portfolio evidence records this non-fork public repository as updated 2025-10-27 and serving `florist.co.id` with HTTP 200. The `syamsulalam/florist.co.id` candidate is an older fork last updated 2024-07-13; `file-wpvivid/backup-florist.co.id` is an older backup.
- The current homepage canonical is `https://florist.co.id`. The repository workflow derives canonical hostnames from the repository name, and `.clients` points customer contact links to `klik.florist.co.id`.
- The static WordPress export contains 15,584 tracked files. The audit used git-tree metadata and a narrow sparse checkout; bulk city and media files were not materialized.
- The generated README declares 7,263 sitemap URLs and contains exactly 7,263 exact, trailing-slash-normalized unique URLs.
- Those 7,263 URLs contain 3,631 root URLs plus 3,632 under `/table-flower/`. After removing the `/table-flower/` prefix, 3,631 nested URLs exactly mirror all 3,631 root URLs; the one additional nested URL is the `/table-flower/` hub itself.
- The root set contains 2,945 product/service-location URLs: 491 each for table flower, standing flower, paper flower board, flower board, and event styling, plus 490 hand-bouquet URLs.
- The root set also contains 74 `/bunga/` flower/entity URLs, 293 `/berita/` archive and pagination URLs, 300 `/category/` archive and pagination URLs, and 19 core/utility URLs.
- `page-sitemap.xml` contains 29 page routes, including product hubs, 12 flower-board use/material pages, shop/cart/checkout/account, company/contact, and service pages. `category-sitemap.xml` contains 35 category routes. These smaller sitemaps do not reconcile cleanly with the generated 7,263-URL list.
- Sampled core pages confirm commercial coverage for flower boards, standing flowers, table flowers, hand bouquets, paper flower boards, event styling, fresh-flower/design/custom-order/delivery services, company information, and contact.
- The homepage and several product pages use claims such as “#1”, “terbaik”, “murah”, “100%”, “12+”, rapid delivery, and nationwide delivery. The repository audit does not substantiate those claims.
- `/bunga-papan/` and `/flower-boards/` have substantially overlapping product/H1 intent. `/shop/` contains no product links or visible price markers in the audited static snapshot.
- Botanical routes include inconsistent spelling/taxonomy and malformed paths such as `/bunga/Jamesonii)/`; `garbera` and `gerbera` variants also appear.

Counts describe repository and sitemap evidence, not live inventory, indexation, order capability, delivery coverage, botanical correctness, product safety, or commercial performance.

## Existing coverage and risks

| Existing URL/pattern | Observed role/problem | Decision | Destination/owner | Verification needed |
|---|---|---|---|---|
| `/` | Commercial overview mixes services, product choices, process, and unsupported superlatives | keep | Homepage owns brand/service overview; `panduan-memesan-bunga-dari-florist` owns the educational entry path | Verify live offers, trust metrics, testimonials, service claims, and canonical |
| `/table-flower/` | Legitimate table-arrangement hub also becomes the parent of a duplicate site tree | keep | Keep the hub; remove the accidental role as alternate root for unrelated routes | Verify current internal links, canonical tags, GSC signals, and deployment rewrites |
| `/table-flower/<every-root-route>` | 3,631 nested URLs mirror every root URL after prefix removal | redirect | Redirect each mirror to its root equivalent except the `/table-flower/` hub | Crawl response/canonical parity, backlinks, traffic, and query history before rollout |
| `/jual-table-flower-<place>`, `/jual-standing-flower-<place>`, `/jual-paper-flower-board-<place>`, `/jual-handbouquet-<place>`, `/jual-flower-board-<place>`, `/jasa-styling-event-<place>` | 2,945 root location pages form six large service-area matrices; local value is not established by route names | manual review | Keep only pages with verified local stock/partner, product scope, cutoff, fee, delivery evidence, or substantive local constraints | Sample content hashes, partner records, actual order coverage, GSC traffic/leads, and route truth |
| `/berita/` and 292 related archive/pagination entries | Archive is dominated by location/service posts rather than a curated learning path | noindex | Maintained topic hubs and article pages own discoverable editorial intent | Confirm crawl paths, article indexation, traffic, and pagination implementation |
| `/category/` and 299 related archive/pagination entries | 35 category entities expand into a large archive/pagination footprint with overlapping product and occasion terms | merge | Retain a small reader-facing taxonomy; noindex thin/paginated archives without canonicalizing every page to page one | Map article ownership, backlinks, internal discovery, and archive content uniqueness |
| `/bunga/` | 74 flower/entity routes mix common/scientific names, variant levels, misspellings, and malformed paths | merge | Build verified flower-family hubs and redirect duplicates/misspellings to the accepted entity owner | Check accepted names, synonyms, content quality, links, and query history with botanical review |
| `/bunga/Jamesonii)/`, `garbera`/`gerbera` variants | Malformed or inconsistent botanical routing | redirect | Correct accepted entity route or remove when no useful history exists | Verify intended species/entity, backlinks, GSC queries, and final botanical owner |
| `/bunga-papan/` and `/flower-boards/` | Both own “Jasa Flower Boards” intent | merge | Select one canonical commercial hub; preserve the stronger URL and redirect the other | Compare backlinks, leads, content, internal links, and live canonicals |
| Flower-board use/material pages under `/bunga-papan/*` | Useful product distinctions, but some occasion and material pages may overlap category archives and articles | expand | Commercial/product pages own purchasable forms; FLS-07 and FLS-10 knowledge pages own craft/material and occasion education | Verify actual offered construction, product photos, availability, and route intent |
| `/standing-flower/`, `/handbouquet/`, `/paper-flower-board/`, `/styling-event/` | Clear product/service hubs with repeated unsubstantiated “100%/12+” blocks and broad coverage claims | expand | Hubs own current offers; relevant knowledge clusters own selection, craft, care, safety, and procurement | Substantiate metrics, inventory, team experience, geography, and original project/product evidence |
| `/layanan/` | Broad fresh flower, design, custom order, and fast-delivery promise | expand | Service overview remains commercial; FLS-11, FLS-13, and FLS-15 own order, availability, and delivery education | Verify response/cutoff/delivery process, substitutions, complaints, and fresh-flower handling |
| `/shop/`, `/cart/`, `/checkout/`, `/my-account/` | WooCommerce utility routes exist, but the static `/shop/` snapshot exposes no products or prices | manual review | Keep only if commerce functions live; otherwise remove from index and route buyers to a verified ordering flow | Test live catalog, cart, payment, privacy, confirmation, stock, taxes/fees, and account handling |
| `/wp-admin/`, `/feed/`, `/author/`, `/404/`, `/1162-2/`, `/sample-page/`, `/hello-world` | Utility, archive, placeholder, or legacy URLs appear in the generated sitemap | remove | Exclude from XML sitemap; redirect useful legacy URLs, return correct 404/410 for abandoned placeholders | Check response codes, backlinks, internal links, and any legitimate content |
| Homepage, product, and service claims | “#1”, “terbaik”, “murah”, “100%”, “12+”, fast delivery, and nationwide reach are not substantiated by repository evidence | manual review | Replace with specific, dated, provable service evidence or remove | Source records, order coverage, staff tenure, service-level data, testimonials, and legal review |
| `README.md`, page/category sitemaps, and sitemap files | Inventories disagree in route scope and duplicate structure | canonicalize | Generate one XML sitemap set containing only final canonical, indexable, 200-status URLs | Full crawl, sitemap-source audit, deployment routing, and resubmission in Search Console |

## Coverage matrix

| Completeness lens | Topic owners | Coverage decision |
|---|---|---|
| Definition, vocabulary, taxonomy, and history | FLS-01, FLS-02 | Distinguish florist, floristry, product form, flower entity, cultivar, common/scientific name, and commercial grade |
| Anatomy, materials, mechanics, and measurement | FLS-03, FLS-07, FLS-08 | Explain stems, focal/filler/line/foliage roles, mechanics, dimensions, balance, water source, support, and installation interfaces |
| Need, survey, requirements, selection | FLS-04 through FLS-11 | Start from recipient, occasion, message, display environment, timing, budget, sensitivities, and delivery constraints |
| Budget and procurement | FLS-11, FLS-12 | Order briefs, quote comparison, substitution, proof approval, fees, scope, and cancellation have distinct owners |
| Preparation and creation | FLS-03 through FLS-08 | Craft guidance defines tools, conditioning, mechanics, assembly, quality checkpoints, and stop conditions |
| Handover, display, and use | FLS-14, FLS-15 | Receipt inspection, placement, hydration, environment, delivery proof, and recipient coordination are explicit |
| Inspection, maintenance, troubleshooting | FLS-13, FLS-14 | Freshness selection, vase life, wilting, water problems, mold, pet/child exposure, and disposal have clear paths |
| Replacement, reuse, and end-of-life | FLS-14, FLS-17 | Refresh, redesign, dry/preserve when appropriate, reuse mechanics, segregate waste, and dispose responsibly |
| Stakeholder and venue context | FLS-04 through FLS-10, FLS-15, FLS-16 | Buyer, recipient, bereaved family, couple, corporate approver, venue, hospital, food service, pet owner, and florist needs differ |
| Climate, geography, and availability | FLS-02, FLS-13, FLS-15 | Tropical heat, humidity, rain, distance, season, cold chain, and local supply change substance; city-name swapping does not |
| Quality levels and alternatives | FLS-02, FLS-04 through FLS-08, FLS-12 | Compare flower/foliage mix, size, mechanics, finish, lifespan, service scope, and alternatives without equating high price with quality |
| Safety and health | FLS-03, FLS-08, FLS-16 | Cutting tools, wire, pins, unstable installations, sap, pollen, fragrance, ingestion, pets, children, food, and venue restrictions receive evidence gates |
| Failure modes | FLS-08, FLS-13, FLS-14, FLS-15, FLS-18 | Collapse, wilt, breakage, browning, water loss, mold, heat damage, late delivery, wrong message, and substitution are mapped to controls |
| Standards, regulation, and evidence | FLS-12, FLS-15 through FLS-18 | Verify consumer, privacy, payment, venue, plant-health/import, safety, and environmental claims with current primary sources before publication |
| Environmental impact | FLS-02, FLS-07, FLS-13, FLS-15, FLS-17 | Sourcing, seasonality, refrigeration, transport, floral foam, frames, plastic, water, chemicals, reuse, and waste are in scope |
| Fundamentals, how-to, comparison, diagnosis | FLS-01 through FLS-18 | Each article owns one reader job and states what it cannot safely or reliably decide |
| Calculators and visual reference | FLS-03, FLS-07, FLS-08, FLS-11, FLS-12, FLS-15 | Brief forms, dimension diagrams, recipe/quantity ranges, quote tables, packing layouts, and checklists expose assumptions |
| Case studies | FLS-04 through FLS-10, FLS-15, FLS-18 | Publish only from permissioned, dated orders/events with brief, constraints, substitutions, delivery, result, and original images |
| Commercial support | FLS-11, FLS-12, FLS-15, FLS-18 | Neutral education prepares a buyer; product/service routes retain availability, quote, checkout, and booking intent |
| News and trends | FLS-02, FLS-03, FLS-17, FLS-18 | Cover durable material, sourcing, style, delivery, and craft changes only when sourced and maintainable |

## Topical map

| Topic ID | Parent topic | Reader outcome | Required subtopics/questions | Evidence/formats | Boundary | Article target |
|---|---|---|---|---|---|---:|
| FLS-01 | Florist fundamentals, vocabulary, and product taxonomy | Readers can name the service/product they need without confusing flowers, arrangement forms, occasions, or delivery services | Florist versus flower shop versus decorator; cut flower versus potted/dried/artificial; bouquet, hand bouquet, table flower, standing flower, wreath, flower board; focal/filler/line/foliage; stem count versus visual volume; florist workflow; Indonesian/English terms | Illustrated taxonomy; bilingual glossary; annotated product silhouettes; florist review | Does not recommend a product for an occasion; FLS-04 through FLS-10 own selection and commercial hubs own live offers | 6 |
| FLS-02 | Flower and foliage entities, seasonality, and substitution | Buyers can compare flower families by visual role, handling, availability, sensitivity, and acceptable alternatives | Accepted/common names; cultivar versus species; color/form; stem strength; fragrance; pollen/sap; vase-life variables; local/imported; seasonality; substitution logic; foliage; dried/artificial alternatives; botanical corrections | Verified entity cards; botanical sources; supplier availability records; comparison table; florist/botanist review | Does not diagnose poisoning/allergy or promise stock; FLS-16 owns safety and product routes own current inventory | 6 |
| FLS-03 | Floral design principles, mechanics, tools, and recipes | Readers can understand how a stable, intentional arrangement is designed and documented | Brief; line/form/space; balance; rhythm; proportion; color; texture; focal hierarchy; mechanics; water source; stem preparation; recipe/quantity range; cutting tools; wire/pins/foam alternatives; quality control | Design diagrams; recipe sheet; original build photos; tool-safety checklist; florist review | Does not provide an event installation method or product quote; FLS-08 owns installation and FLS-12 owns pricing | 6 |
| FLS-04 | Hand bouquets and personal gifting | Buyers can choose and receive a hand bouquet suited to recipient, carrying, message, environment, and budget | Bouquet forms; scale; flower/foliage mix; wrapping; grip/weight; fragrance/pollen; water source; travel; presentation; gift note; care handoff; alternatives | Form comparison; recipient brief; dimension photos; care card; florist review | Does not own all gift etiquette or delivery; FLS-10 owns message/occasion and FLS-15 owns delivery | 6 |
| FLS-05 | Table flowers and interior arrangements | Buyers can specify a table arrangement that fits sightlines, surface, duration, food, lighting, air-conditioning, and maintenance | Centerpiece versus side/console/reception; dimensions; sightline; vessel; water; table load; candle/electrical interface; food proximity; scent/pollen; daily refresh; multi-table consistency | Table elevation diagrams; venue checklist; recipe range; original photos; venue/florist review | Does not plan full event styling or food-safety policy; FLS-08 owns event systems and FLS-16 owns exposure constraints | 6 |
| FLS-06 | Standing flowers, wreaths, condolence forms, and ceremonial displays | Buyers can distinguish upright/ceremonial forms and specify stability, message, viewing, venue, and lifecycle | Standing flower; wreath; sympathy form; opening/congratulation display; frame; base; water; dimensions; wind/traffic; sign/message; transport; setup; handover; removal | Form/anatomy diagrams; stability checklist; message proof; florist/event review | Does not own flower-board construction or condolence etiquette; FLS-07 owns boards and FLS-09 owns sympathy context | 6 |
| FLS-07 | Flower boards, substrates, printing, and reusable structures | Buyers and makers can compare board systems by finish, stability, weather, message, materials, transport, reuse, and waste | Conventional board; paper flower board; acrylic; cardboard; plywood; styrofoam; printing; frame/base; lettering; attachment; wind/rain; dimensions; proofing; assembly; reuse; disposal | Material matrix; section/detail diagrams; original build photos; stability/waste review | Does not choose wording or approve an installed structure; FLS-10 owns message and FLS-08 owns site installation | 6 |
| FLS-08 | Wedding and event floral styling | Event teams can translate concept, venue, schedule, guest flow, safety, and budget into a coordinated floral scope | Ceremony/reception; stage; aisle; entrance; photo area; table; ceiling/overhead boundary; load-in; mechanics; utilities; candles; egress; weather; mock-up; installation; strike; contingency; vendor interfaces | Venue survey; mood board; scope matrix; run sheet; installation hold points; florist/event/K3 review | Does not replace event planning, structural/rigging approval, or venue authorization; commercial `/styling-event/` owns booking | 6 |
| FLS-09 | Sympathy, funeral, memorial, and sensitive delivery | Buyers can send appropriate flowers with respectful language, timing, venue coordination, and recipient privacy | Condolence forms; faith/cultural preferences; family/venue contact; name/title verification; message tone; timing; hospital/funeral-home/cemetery rules; delivery proof; alternatives; removal/donation | Etiquette decision tree; message checklist; venue-call script; cultural/faith review | Does not declare one universal religious custom or give grief counseling; FLS-10 owns general wording and FLS-15 owns delivery mechanics | 6 |
| FLS-10 | Occasions, symbolism, color, and message etiquette | Buyers can match arrangement, palette, symbolism, and wording to a specific relationship and occasion without relying on rigid myths | Birthday; anniversary; wedding; graduation; opening; congratulations; apology; thank-you; religious holidays; corporate protocol; color meanings as context-dependent; names/titles; bilingual message; prohibited/ambiguous wording | Occasion matrix; message templates with review notes; cultural sources; proof checklist | Does not promise a flower has one universal meaning or own sympathy depth; FLS-09 owns bereavement and FLS-11 owns order approval | 6 |
| FLS-11 | Order brief, customization, proofing, and substitution approval | Buyers can provide complete requirements and approve changes before production | Recipient; occasion; product/form; size; palette; preferred/prohibited flowers; sensitivities; message; budget; deadline; venue; access; delivery contact; photo expectation; substitution tiers; proof; change log; acceptance | Order-brief template; proof checklist; substitution matrix; RACI; florist review | Does not quote price or promise stock/delivery; FLS-12 owns quote structure, FLS-13 availability, and FLS-15 delivery | 6 |
| FLS-12 | Pricing, budget, quotation, payment, and consumer terms | Buyers can understand cost drivers and compare quotes with the same scope and risk | Flower/foliage mix; size/recipe; mechanics/vessel/frame; labor; design; transport; setup/strike; urgency; season; waste; tax/fees as stated; deposit; change/cancel/refund; damage; quote validity; proof; invoice | Cost-component table; quote-comparison sheet; scenario ranges without market claims; legal/accounting review | Does not publish universal prices or legal/financial advice; product routes own dated quotes and FLS-13 owns stock uncertainty | 6 |
| FLS-13 | Sourcing, availability, freshness, quality, and procurement | Buyers and florists can assess what is realistically available and recognize fresh, damaged, or unsuitable material | Local/imported supply; season; market/supplier lead time; harvest/cold chain; grade; stem/bloom/foliage condition; pests/disease signs; hydration; substitution; rejection; traceability; ethical claims | Receiving checklist; defect photo atlas; supplier confirmation log; botanical/plant-health/florist review | Does not promise stock, certify plant health, or diagnose human exposure; FLS-02 owns entities and FLS-16 owns health safety | 6 |
| FLS-14 | Conditioning, display care, vase life, and troubleshooting | Recipients and venue teams can inspect, condition, display, refresh, and retire arrangements safely | Clean tools/vessels; recut; hydration; water hygiene; temperature; light; airflow; fruit/ethylene; feeding claims; foam/water source; top-up; droop/browning/mold/odor; refresh; drying/preservation boundary; disposal | Care cards by product; symptom decision tree; time-lapse/original photos; florist/horticulture review | Does not provide medical treatment, pesticide use, or guarantee vase life; FLS-16 owns exposure and FLS-17 owns disposal | 6 |
| FLS-15 | Packaging, delivery, cold chain, setup, and proof of receipt | Buyers can plan a delivery that protects the arrangement and reaches the right person/venue at the right time | Packaging; hydration; temperature; vehicle placement; route/time buffer; rain/heat; access; recipient call; privacy; hospital/hotel/office/funeral/event rules; failed delivery; condition photos; setup; proof; claims | Packing diagrams; delivery checklist; chain-of-custody log; venue matrix; operations review | Does not guarantee nationwide/same-day service or publish city pages; live service routes own verified coverage and quote | 6 |
| FLS-16 | Toxicity, allergy, pets, children, food, and venue safety | Buyers can identify exposure questions, select lower-risk options with professional input, and know when to stop and seek expert help | Ingestion; sap/skin; pollen; fragrance; thorns; pets; children; food/cake/table; hospital/care setting; religious/venue restrictions; pesticide residue; mislabeled species; symptoms; emergency information; safer placement/alternatives | Exposure checklist; authoritative toxicology/veterinary sources; species verification; medical/veterinary/food-safety review | Does not label an arrangement “safe”, “non-toxic”, or “hypoallergenic”, diagnose symptoms, or give treatment; emergency/professional services own response | 6 |
| FLS-17 | Sustainable floristry, sourcing claims, reuse, and waste | Buyers and florists can compare environmental claims by defined boundaries and choose practical reduction/reuse paths | Local versus imported trade-offs; season; certification/traceability; refrigeration/transport; water/chemicals; floral foam; plastic; paper; frames/vessels; rentals; reusable mechanics; donation; compost boundary; mixed/hazardous waste; claim verification | Lifecycle boundary map; material-flow diagram; supplier evidence; waste audit; environmental review | Does not claim “eco-friendly”, “zero waste”, or lower carbon without defined evidence; FLS-12 owns price and FLS-13 owns availability | 6 |
| FLS-18 | Florist operations, quality assurance, portfolio evidence, and service recovery | Florist teams can build repeatable work from inquiry through post-delivery learning without fabricating authority | Intake; design/recipe; procurement; conditioning; production; QC; message proof; packing; delivery; installation; photo consent; privacy; defects; complaint triage; remake/refund boundary; supplier/vendor records; case-study evidence; KPI | SOP map; QC checklist; defect log; case-study template; privacy/legal/operations review | Does not claim certification, experience, or performance without records; commercial routes own offers and FLS-12 owns customer terms | 6 |

## Related-domain opportunities

- `Floral.id` may independently cover the same flowers, craft, commerce, and partner ecosystem. `Florist.co.id` should maintain its buyer-to-recipient and direct florist-service path; overlap across the two domains is not cannibalization.
- `WeddingEvent.co.id` can cover full wedding/event planning and vendor orchestration while FLS-08 explains floral scope and installation interfaces.
- `Suvenir.id` may cover non-floral gifts and keepsakes; contextual comparison is useful when a recipient or venue makes flowers unsuitable.
- `Katering.co.id` can own food production and service safety. FLS-05/FLS-16 cover only the floral proximity and venue-interface problem.
- Cross-domain links must help a reader complete a task. Ownership does not justify a sitewide portfolio link network.

## Consolidation plan

1. Crawl all 7,263 generated sitemap URLs with response, final URL, canonical, title, H1, word count, content hash, indexability, and internal inlinks.
2. Preserve `/table-flower/` as the commercial table-arrangement hub. Redirect its 3,631 mirrored descendants to the equivalent root URLs after verifying parity, backlinks, and GSC signals.
3. Audit the 2,945 root location pages in six product/service families. Keep only pages backed by real local inventory/partner/service capability, current cutoff/fee, delivery process, and unique constraints; consolidate or noindex weak copies after measuring traffic and leads.
4. Reconcile the README inventory, XML sitemap index, page sitemap, category sitemap, and deployed routes. Publish only final canonical, indexable, 200-status URLs in XML.
5. Merge `/bunga-papan/` and `/flower-boards/` after selecting the stronger historical/commercial URL. Preserve useful content and route signals.
6. Rebuild `/bunga/` into verified entity/family hubs. Correct malformed names, accepted-name/synonym relationships, and unsafe toxicity/allergy claims before redirects.
7. Reduce 300 category and 293 news/archive routes to a small task-oriented taxonomy. Noindex paginated/thin archives while preserving crawlable article discovery.
8. Remove utility, placeholder, and admin URLs from sitemaps. Test `/shop/`, cart, checkout, account, payment, privacy, confirmation, and inventory before exposing commerce routes to search.
9. Replace unsubstantiated superlatives, percentages, tenure, speed, and nationwide claims with dated operational evidence or remove them.

## Internal-link architecture

- `panduan-memesan-bunga-dari-florist` is the central editorial hub. It links to all 18 parent hubs and to commercial product/service routes only when the reader has enough information to act.
- Reader path: FLS-01 terminology → FLS-02 flower/availability → FLS-04 through FLS-10 product/occasion → FLS-11 brief → FLS-12 quote → FLS-15 delivery → FLS-14 care.
- Safety path: every flower/product/entity page links to FLS-16 when pets, children, ingestion, sap, pollen, fragrance, thorns, food, or venue restrictions may matter. It must not display a generic “safe” badge.
- Craft path: product-form pages link to FLS-03 principles; boards link to FLS-07; installations link to FLS-08; failure/maintenance links to FLS-14 or FLS-18.
- Procurement path: FLS-11 and FLS-12 link to FLS-13 for availability/substitution and FLS-17 for material/sourcing evidence. Current commercial pages receive links only from relevant buyer decisions.
- Diagnostic pages in FLS-14 link backward to freshness/conditioning in FLS-13, forward to replacement/disposal in FLS-17, and to FLS-16 for exposure concerns.
- Every article links upward to its topic hub; every hub links to all six children. Related links follow the specific lifecycle step and are not copied as one generic block.

## Evidence and editorial standards

1. Separate repository observation, botanical fact, supplier statement, florist judgment, customer preference, and editorial hypothesis.
2. Verify common/scientific names and synonyms against current authoritative botanical databases. A cultivar, hybrid, trade name, and species are not interchangeable.
3. Toxicity, allergy, medical, veterinary, food-contact, and hospital claims require correctly identified material and current authoritative toxicology/medical/veterinary/venue evidence. Never call a flower “safe”, “non-toxic”, or “hypoallergenic” without a defined subject, exposure, and qualified review. Provide stop/seek-help guidance, not diagnosis or treatment.
4. Availability, seasonality, color, stem length, grade, and substitution claims require dated supplier or receiving evidence. Product pages disclose that natural materials vary.
5. Prices and delivery promises are dated offers, not evergreen facts. State inclusions, exclusions, substitution rules, fee/cutoff basis, quote validity, and confirmation point. Never invent nationwide coverage or same-day capability.
6. Craft instructions identify sharp tools, wire/pins, unstable frames, overhead work, candles/electrical interfaces, lifting, egress, and venue approval. High-risk installation belongs to trained teams and competent structural/rigging specialists where applicable.
7. Sustainability claims define their boundary and evidence: source, certification/traceability, transport/refrigeration, mechanics, packaging, reuse, and end-of-life. “Eco-friendly”, “biodegradable”, “local”, and “zero waste” require proof.
8. Original product/event photos record date, brief, substitutions, approximate dimensions, environment, delivery/setup state, and permission. Stock photos do not prove inventory, craft, or experience.
9. Case studies require a real permissioned order, constraints, scope, quote boundary, substitutions, delivery/setup evidence, result, limitations, and no fabricated testimonial.
10. Consumer, privacy, payment, cancellation/refund, plant-health/import, venue, safety, and environmental statements are checked against current primary sources and qualified review before publication; no unverified clause numbers.

## First bounded publication cluster

Wave `W1-buyer-safe-order` contains 12 assets:

1. FLS-01-01 — central florist-ordering guide.
2. FLS-01-02 — product-form taxonomy.
3. FLS-02-01 — flower selection and substitution framework.
4. FLS-03-01 — design-brief fundamentals.
5. FLS-04-01 — hand-bouquet selection.
6. FLS-06-01 — upright/ceremonial-form comparison.
7. FLS-11-01 — complete order brief.
8. FLS-12-01 — price-component explanation.
9. FLS-13-01 — freshness and receiving inspection.
10. FLS-15-01 — delivery-information checklist.
11. FLS-16-01 — exposure and safety screening.
12. FLS-17-01 — practical lower-waste selection.

The cluster lets a buyer identify the product, choose materials and design, document the order, understand cost and substitution, screen safety, receive a viable arrangement, and consider end-of-life. It creates a useful path before expanding occasion and craft depth.

Monitor final-canonical indexation, impressions by distinct intent, order-brief completion, clicks from education to the correct product hub, substitution/clarification rate, qualified inquiries, delivery complaints, care-page engagement, and GSC evidence of same-domain query overlap. Ranking alone is not success.

## Definition of done

- All 18 parent topics and 108 article briefs have a published or explicitly deferred owner.
- The 3,631 accidental `/table-flower/` mirrors are consolidated without deleting the legitimate hub.
- Location pages survive only when real local capability and unique value are verified; place-name substitution is not completion.
- Botanical identity, toxicity, allergy, food/venue, sustainability, price, availability, and delivery claims pass their evidence gates.
- Product/service routes own live offers; educational articles own one bounded reader job; no two `Florist.co.id` pages equally satisfy the same query.
- XML sitemaps contain only final canonical, indexable, 200-status URLs; utility, placeholder, malformed, and thin archive URLs are resolved.
- Publication metrics include indexation, task completion, qualified inquiries, order clarity, substitutions/complaints, and cannibalization—not content volume or ranking alone.
