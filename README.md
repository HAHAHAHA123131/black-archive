# THE BLACK ARCHIVE

**An evidence-tiered index of the CIA's deepest programs — from Mockingbird and MKUltra to black sites, coups and claims that leave no paper trail.**

**Live:** https://hahahaha123131.github.io/black-archive/ · **Repository:** https://github.com/HAHAHAHA123131/black-archive

A single-file, zero-dependency static website (~196 KB). Pure black and white, no build step, no tracking, no frameworks — and **zero external requests**: even the fonts (Archivo and IBM Plex Mono, SIL Open Font License 1.1) are embedded directly in `index.html`, so the page contacts nothing but its own host when you load it.

---

## What's inside

| Section | Contents |
|---|---|
| **§ 00 Tiers** | How the four evidence tiers work — Confirmed / Studied / Unconfirmed / Unknown |
| **§ 01 Timeline** | 28 milestones, 1946 → 2024, horizontally scrollable |
| **§ 02 Programs** | 24 program files across two volumes, filterable and searchable |
| **§ 03 Named subjects** | 14 people — confirmed, disputed and alleged, each with sources |
| **§ 04 Connections log** | 15 tiered ties between the Agency and companies, brands and names |
| **§ 05 Method** | Sourcing rules, tiering rules and the limits of the archive |

**Volume I** — MKUltra, Operation Mockingbird, Operation CHAOS, Operation Midnight Climax, Project ARTICHOKE, the Guatemala experiments, Operation TPAJAX, extraordinary rendition & black sites, Project Stargate, Operation Northwoods, MKNAOMI, Project Azorian, the Contra–cocaine allegations, the JFK assassination investigations, and three claim-only/unknown entries (post-1973 MKUltra, modern Mockingbird, crash-retrieval claims, Montauk, Blue Beam).

**Volume II** — The Family Jewels, Operation PBSUCCESS, the CIA–Mafia assassination plots, Operation Mongoose.

**Connections log** — Mockingbird-era newsrooms, In-Q-Tel → Keyhole → Google Earth, Amazon Web Services, Microsoft/Google/Oracle, Booz Allen Hamilton, ITT, BCCI, the Congress for Cultural Freedom, Palantir, the Maxwell family, SpaceX/NRO, and claim-only entries for Jeffrey Epstein, BlackRock, Vanguard and the Rothschild family.

---

## Evidence tiers

- **Confirmed** — established by declassified records, official admissions, court judgments or congressional investigation.
- **Studied** — documented, but its findings, scope or conclusions are disputed, partially redacted or under official review.
- **Unconfirmed** — widely claimed; no credible public evidence. Recorded as claim, not fact.
- **Unknown** — no official record exists either way.

The same rule applies to the connections log: a contract or a filing is evidence; a customer relationship is not ownership; where only a claim exists, only the claim is recorded.

---

## Run it

```bash
# open directly
open index.html            # macOS
xdg-open index.html        # Linux

# or serve it
python3 -m http.server 8000
```

No dependencies. Everything (HTML, CSS, JS, data) lives in `index.html`.

## Project structure

```
black-archive/
├── index.html   # the whole archive: markup, styles, data, behaviour
├── README.md
└── LICENSE
```

## Contributing

1. Fork / copy the repo.
2. New program? Add an `<article class="record">` with `data-cat` set to one of the four tiers, a `FILE NN` index, and a `Sources` list.
3. New subject? Add a `<div class="vic">` with `data-cat` of `confirmed`, `disputed` or `alleged`.
4. Cross-links live in the `XLINKS` map inside the `<script>` block — `file-NN` ↔ `s-NN` with a reason string.
5. **Never upgrade a claim.** An entry moves up a tier only when a primary record, judgment or official admission exists.

## Sourcing rules

Primary sources first: declassified FOIA material, Senate reports, court rulings, official investigations. Wikipedia links are navigation aids, not authorities. Every entry carries its own citation list (136 citations in total). If a source contradicts an entry here, trust the source.

## License

MIT — see [LICENSE](LICENSE). Attribution to original sources is required when reusing individual entries; citations remain theirs.

*Educational index compiled from open sources. No classified material. No claim of ongoing illegality is made where evidence does not exist.*
