# CUWB Mock Site

A mock marketing site for [CUWB.io](https://www.cuwb.io/) — Ciholas's Ultra-Wideband real-time location system product. The site demonstrates what a content-depth and SEO authority strategy could look like for CUWB, based on the audit documented in [content-seo-cuwb.md](./content-seo-cuwb.md).

The central argument of that audit: CUWB's technical substance is real, but it is packaged as product pages and documentation rather than as pages that match how buyers discover, compare, and justify RTLS purchases. This mock site builds out the missing content architecture — learn guides, technology comparisons, solution pages, deployment planning, and competitor comparison pages.

## What this is

This is a **Next.js static mock site**, not connected to any CMS, backend, or real CUWB systems. All content is hardcoded and representative. It is a working prototype for evaluating page structure, information architecture, and content strategy — not a production codebase.

## Site structure

### Product pages
Core hardware and software product pages, mirroring what CUWB already publishes:

| URL | Description |
|-----|-------------|
| `/anchors` | UWB anchor hardware |
| `/tags` | UWB tag hardware |
| `/software` | Local RTLS software and API |
| `/accessories` | Mounts, kits, and deployment accessories |
| `/custom-uwb` | Custom UWB engineering and OEM services |
| `/pricing` | Hardware pricing and no-recurring-fee positioning |

### Learn / pillar content
Educational pages targeting informational and consideration-stage search queries — the biggest gap on the real site:

| URL | Description |
|-----|-------------|
| `/learn/uwb-rtls` | What is UWB RTLS? How does it work? |
| `/learn/indoor-asset-tracking` | Indoor asset tracking overview |
| `/learn/uwb-vs-ble-rfid-gps` | Technology comparison hub |
| `/learn/uwb-vs-ble` | UWB vs Bluetooth RTLS deep dive |
| `/learn/uwb-vs-rfid` | UWB vs RFID asset tracking |
| `/learn/uwb-vs-gps-indoor` | UWB vs GPS for indoor tracking |
| `/learn/uwb-vs-wifi-positioning` | UWB vs Wi-Fi positioning |
| `/learn/local-rtls-vs-cloud-rtls` | Local RTLS vs cloud RTLS |
| `/uwb` | UWB technology overview (existing CUWB page) |

### Solution / use-case pages
Industry and workflow pages that match how buyers search when they already know the category:

| URL | Description |
|-----|-------------|
| `/solutions/warehouse-asset-tracking` | Warehouse asset and forklift tracking |
| `/solutions/manufacturing-rtls` | Manufacturing floor RTLS |
| `/solutions/work-in-progress-tracking` | WIP and fixture tracking |
| `/solutions/forklift-tracking` | Forklift and vehicle tracking |
| `/solutions/robotics-agv-tracking` | Robotics and AGV localization |
| `/solutions/hospital-equipment-tracking` | Healthcare asset tracking |
| `/solutions/sports-athlete-tracking` | Sports and performance tracking |
| `/solutions/mining-personnel-tracking` | Mining personnel and equipment |

### Deployment planning hub
A cluster of practical planning pages targeting buyers who are actively sizing a system:

| URL | Description |
|-----|-------------|
| `/rtls-deployment-planning` | Hub: planning a UWB RTLS deployment |
| `/rtls-deployment-planning/uwb-network-requirements` | Network and infrastructure requirements |
| `/rtls-deployment-planning/how-obstructions-affect-uwb` | How metal, walls, and NLOS affect UWB |
| `/rtls-deployment-planning/estimate-tag-count-and-rate` | How to size tag count and update rate |
| `/rtls-deployment-planning/indoor-vs-outdoor-uwb-deployment` | Indoor vs outdoor deployment considerations |
| `/rtls-deployment-planning/rtls-commissioning-checklist` | Pre-deployment checklist |
| `/learn/uwb-anchor-placement` | UWB anchor placement guide |

### Competitor comparison pages
Decision-stage pages for buyers who are actively shortlisting vendors:

| URL | Description |
|-----|-------------|
| `/compare` | Comparison hub |
| `/compare/cuwb-vs-pozyx` | CUWB vs Pozyx |
| `/compare/cuwb-vs-sewio` | CUWB vs Sewio |
| `/compare/cuwb-vs-kinexon` | CUWB vs KINEXON |
| `/compare/cuwb-vs-ubisense` | CUWB vs Ubisense |
| `/compare/cuwb-vs-redpoint` | CUWB vs Redpoint |
| `/compare/cuwb-vs-wiser` | CUWB vs WISER |
| `/compare/cuwb-vs-zebra` | CUWB vs Zebra |
| `/compare/cuwb-vs-litum` | CUWB vs Litum |

### Case studies
Anonymized proof pages in the format recommended by the audit:

| URL | Description |
|-----|-------------|
| `/case-studies/warehouse-asset-tracking-48-anchors` | 48-anchor warehouse deployment |
| `/case-studies/high-speed-robotics-tracking-100hz` | 100 Hz robotics tracking |
| `/case-studies/medical-equipment-tracking-local-rtls` | Hospital equipment tracking |
| `/case-studies/mine-equipment-personnel-tracking` | Mining deployment |

### Articles (existing CUWB content, reproduced)
| URL | Description |
|-----|-------------|
| `/articles/chainpoe` | ChainPoE installation differentiator |
| `/articles/accuracyprecision` | UWB accuracy and precision explainer |

### Other pages
| URL | Description |
|-----|-------------|
| `/` | Homepage |
| `/cuwb-advantage` | Core commercial argument and differentiators |
| `/rtls-api-integration` | API and integration guide |
| `/faq` | Buyer FAQ |
| `/about` | About Ciholas |
| `/contact` | Contact / book a call |

## Running the site

```bash
cd cuwb
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

```bash
npm run build   # production build
npm run start   # serve the production build
npm run lint    # lint
```

## Tech stack

- [Next.js 16](https://nextjs.org/) (App Router)
- [React 19](https://react.dev/)
- [Tailwind CSS 4](https://tailwindcss.com/)
- TypeScript

## Related files

- [content-seo-cuwb.md](./content-seo-cuwb.md) — the full SEO and content strategy audit this site is based on
- [cuwb/PRODUCT.md](./cuwb/PRODUCT.md) — product and feature notes
- [cuwb/DESIGN.md](./cuwb/DESIGN.md) — design system notes
- [cuwb/AGENTS.md](./cuwb/AGENTS.md) — agent/build notes
