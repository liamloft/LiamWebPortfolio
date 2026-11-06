# Goal

Design and build a personal website homepage for Liam Loftus that shows his current work at Rivian, the communities he founded, and the things he builds for fun.

The page should feel like a polished personal field notebook for someone who builds, ships, and runs. It should be professional enough for recruiters and partners, but personal enough to feel written by one person.

Live page: https://claude.ai/artifact/GaVafD6RRSm9Cq8cXviEPC

# Primary Message

## Creativity is intelligence having fun.

Sr. Embedded Software Engineer at Rivian. Former collegiate athlete, founder of Huntington Run Club, and maker with builds like an FPV drone and a 3D printer.

# Content Requirements

## Hero

- Label (mono, uppercase): **Ideas & Notes, 2026 · Southern California**
- Headline, on three lines: **Creativity is / intelligence / having fun.** The last line carries a hand-drawn accent underline.
- Lead: "**Sr. Embedded Software Engineer at Rivian.** Former collegiate athlete, founder of Huntington Run Club, and maker with builds like an FPV drone and a 3D printer."
- Handwritten margin note with a small hand-drawn arrow: *note to self: try it. it's usually not as hard as you think, and if it is, great!*
- Calls to action that jump to sections: **See the work ↓** (primary button) and **Side quests ↓** (text link)
- Accent color picker labeled **Ink**
- Hand-drawn pier sketch, captioned **fig. 1 · the view from the pier**

## Now Strip

- Currently building the **Rivian Adventure Network** (RAN) at Rivian. The network name links to https://rivian.com/experience/charging
- Founder, **Huntington Run Club** & **Social Plunge**. Each name links to its Instagram page: instagram.com/huntingtonrunclub and instagram.com/socialplunge
- **Seeking ambitious ideas →** links to mailto:liamloft8@gmail.com

## § 01 Work

Heading: **Chargers, from board to cloud.**
Supporting copy: Six years across test hardware, factory automation, and the DC fast charging network.

Stat cards (the numbers are prominent):

- **$10M+**: in kWh delivered on the RAN DCFC platform I develop software for
- **98%**: uptime across 1000+ plugs
- **+15%**: storefront sales growth, Top 3 on Mercado Libre

Timeline (dates in mono on the left, details on the right):

- **Sr. Embedded Software Engineer**, Rivian, Irvine. Aug 2024 – now.
  - Pitched custom HMI features to senior leadership and led the cross-functional build, mentoring a junior developer. It opened new revenue streams and strategic partnerships.
  - Built cloud integration (OCPP 2.0.1), billing, and HMI software for OpenRAN, Rivian's open DC fast charging network.
- **Embedded Software Engineer**, Rivian. Aug 2022 – Aug 2024.
  - Led credit card reader integration for OpenRAN across cloud and embedded software, legal, finance, the mobile app, and third-party payments.
  - Engineered DCFC embedded systems in C++, Docker, Jenkins, Qt, GitLab, Linux, and Mender.
- **Test Automation Engineer**, Rivian. Feb – Aug 2022.
  - Designed end-of-line ECU test hardware and sequences for the R1T and R1S with NI DAQ, LabVIEW, TestStand, Python, and OpenHTF.
- **Mechatronics Engineer**, Lawrence Equipment, Los Angeles. Feb 2021 – Feb 2022.
  - Installed and serviced automated flatbread and chip fryer production lines worldwide.
  - Programmed Allen-Bradley PLCs (Studio 5000) and designed parts in Autodesk Inventor.
- **Business, Sales & Engineering**, Uría S.A. de C.V., Mexico City. Jun 2020 – Feb 2021.
  - Generated over $500,000 MXN in sales from new customers nationwide.
  - Retrofitted a 1980s ELOX wire EDM machine with a Fanuc 200c control, so it takes USB NC code instead of punched tape.

## § 02 Side quests

Heading: **Things I made because I wanted to.**
Supporting copy: Communities, builds, and one very old machine.

Numbered entries, each with a hand-stamped tag:

1. **Huntington Run Club** (Community). Founded @huntingtonrunclub. Partners have included Red Bull, Electrolit, and TruFru.
2. **Social Plunge** (Community). Founded @socialplunge, with brand partnerships of its own.
3. **FPV drone** (Build). Built a custom first-person-view drone, and I fly it.
4. **3D printer** (Build). Built the printer, then designed and made custom parts on it.
5. **Wire EDM, USB edition** (Retrofit). Brought a 1980s machine into the USB era, then cut die sets on it with Mastercam.

## § 03 About

Heading: **Athlete first.**

- Played football through college on a student-athlete scholarship, and now races triathlons.
- Studied Mechatronics Engineering at Tec de Monterrey, with courses at Sydney, Caltech, and UC Irvine. Speaks English, Spanish, and Russian. Lululemon ambassador.
- Skill chips (mono): C++, Python, Git, SolidWorks, Inventor, Mastercam, 3D print, FPV
- Education list:
  - UC Irvine, Embedded Systems Engineering. 2025
  - Caltech, Object-Oriented Programming. 2021
  - University of Sydney, Quantitative Analysis. 2020
  - Tec de Monterrey, B.S. Mechatronics. 2016–20

## § 04 Contact

Heading: **Got an ambitious idea?**

- Large email link: liamloft8@gmail.com
- Phone: (949) 867-9463
- Instagram: @huntingtonrunclub and @socialplunge

## Footer

Liam Loftus · Sr. Embedded Software Engineer · Rivian · made with care in 2026

# Design Requirements

## Overall Feel

- Personal, warm, and editorial
- A field notebook or annotated portfolio, not a marketing landing page
- Clearly written by one person

## Visual Direction

- Spacious hero with a very large headline
- Dotted-grid paper background with light grain
- Hand-drawn details: the headline underline, the margin-note arrow, the pier sketch, wavy water lines, and hand-stamped tags
- Mono labels for dates, section numbers (§ 01 to § 04), and small text
- Prominent stat cards
- Sections separated by thin rules

## Signature Interaction: the Scroll Line

- A vertical line runs down the left margin and fills with the accent color as the reader scrolls. A droplet at the tip follows the scroll position.
- Each section heading has a ring on the line.
- The line starts at the pier sketch. A short curved connector leaves the left end of the pier and joins the margin line.
- Before the reader scrolls past the pier, the line, droplet, connector, and rings are hidden. They fade in once the reader passes the pier.

## Other Interactions

- Accent color picker with six palettes: Pacific, Sunset, Kelp, Plum, Indigo, and Sand
- The accent choice and the light/dark choice are saved in the browser (localStorage, wrapped in try/catch)
- Hover states on links, buttons, and rows
- Respect reduced-motion preferences

## Theme Support

- Light and dark mode, following the system setting by default, with a manual toggle in the top bar
- All surfaces, text, borders, and accents come from CSS variables, with separate accent values for light and dark so contrast holds in both

## Typography

- Geist for headings and body text
- Geist Mono for dates, labels, notes, and small technical text
- Loaded from Google Fonts, with system fallbacks

## Responsive Behavior

- Works on mobile and desktop
- The timeline, side-quest rows, and About columns collapse to one column on small screens
- Stat cards stack on mobile
- The scroll line gets a narrower margin on mobile
- Safe-area insets are respected on phones

# Implementation Notes

- A single self-contained HTML file with inline CSS and JavaScript, published as a hosted page
- No images; the pier and the underline are inline SVG
- Contact links use mailto: and tel:
- Handles and links to confirm: Instagram handles for both communities

# Open Items

- The Rivian timeline bullets still say "OpenRAN" while the Now strip says "Rivian Adventure Network (RAN)". Decide whether to rename them.
- The browser tab title is still "Liam Loftus: field notes", while the hero label now says "Ideas & Notes".
- The uptime stat shows 98% across 1000+ plugs, while the resume says 97%.
- Confirm the two Instagram handles and the one-line descriptions of the drone and 3D printer builds.
