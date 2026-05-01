---
tags:
  - finance
  - tax
  - serbia
  - capital-gains
  - dandilion
  - private
category: private
created: 2026-05-01
language: en
summary: Action plan for filing Serbian 15% capital-gains tax (PPDG-3R) on the £46,000 Dandilion LLC redemption settlement — covers timing, basis, FX, NBS routing, and U.S. §864(c)(8)/§1446(f) exposure.
---

# Dandilion Settlement — Capital Gains Tax Filing Plan

This note is the operating plan for paying capital-gains tax on the **£46,000 Settlement Amount** received in exchange for redeeming 96 Units of Dandilion LLC. The consultancy (paušalac) side is not in scope here — that has its own filings.

> **TL;DR — what you owe and when**
>
> - **Tax**: Serbian 15% capital-gains tax on the redemption gain. With a near-zero cost basis (the conservative, defensible position), the bill is roughly **£6,900 / ~RSD 970,000** at current FX.
> - **Form**: **PPDG-3R**, filed via [ePorezi](https://eporezi.purs.gov.rs).
> - **Deadline**: **Within 30 days of the Closing date** (the date the 96 Units irrevocably transfer to the Company), reporting the **full £46,000 nominal sale price** in RSD at the NBS middle rate on Closing day. Do NOT wait for the semi-annual stock-account window (that scheme does not apply here).
> - **Single critical decision**: cost basis = 0 (recommended) vs. cost basis = FMV-at-grant (requires amending 2024 filings, usually doesn't pay off). See [§4](#4-the-cost-basis-decision-the-money-question).
> - **Two flags requiring outside advisors before Closing**: U.S. §864(c)(8) ECI/§1446(f) exposure on the LLC side, and Serbian tax treatment of the LLC→Corp conversion of the 95 retained Units.

---

## 1. Deal recap (so the numbers are anchored)

| Item | Value |
|---|---|
| Member | Aleksa Bisercic (Serbian tax resident, in personal name) |
| Company | Dandilion LLC, Delaware (converting to Delaware Corp at/near Closing) |
| Original holding | 191 Units = 21.75% (acquired at LLC formation, **9 Oct 2024**) |
| Redeemed Interest | 96 Units = 50% of holdings = ~10.875% of company |
| Retained after Closing | 95 Units (convert to Corp shares) |
| Settlement Amount | **£46,000** (consideration for the 96 redeemed Units) |
| Payment Plan | 20 × £2,200 + 1 × £2,000, monthly, first installment **1 April 2026** |
| Consultancy termination | 31 January 2026 (separate from the redemption — already handled as paušalac revenue) |
| Tax clause | §9.01 — Member solely responsible for all U.S./state/international taxes |

The redemption (capital event) and the terminated consultancy (income event) are legally and tax-wise separate. This plan covers only the redemption.

---

## 2. Why this is a Serbian capital gain (and only a Serbian capital gain)

Under **ZPDG Article 72**, transfer of "udeo u kapitalu pravnog lica" for consideration is a kapitalni dobitak, taxed under Articles 72–80. Key conclusions from the research:

- **Foreign LLC = treated like Serbian d.o.o. udeo.** ZPDG does not distinguish Delaware LLC from Serbian d.o.o. for individual capital-gains purposes. A Serbian resident is taxed on worldwide capital gains.
- **Redemption (LLC buying back its own units) = sale.** Serbia has no equivalent of U.S. §301/§302 redemption-as-dividend recharacterization. The Settlement Agreement is clean — the £46,000 is consideration for transferred Units.
- **Not paušalac revenue.** The Units are held in your personal name, not by the PR. The redemption gain is reported as an individual on PPDG-3R and does NOT count toward the 6-million-RSD paušalac cap.
- **Not annual GPDG income.** Capital gains are excluded from the godišnji porez na dohodak građana (3× average salary supplementary tax) base under Article 87. So the £46,000 will not push you into GPDG territory.
- **Tax rate**: flat **15%** under Article 87 ZPDG.
- **10-year exemption (Article 72b)**: does NOT apply. Holding period ~16 months.

The only legitimate reclassification risk is if the LLC's 2026 K-1 allocates a chunk of pass-through partnership income (distributive share of profits) to you — that is a dividend-equivalent under Serbian rules, taxed separately. That is unrelated to the Settlement Amount itself; address it when the K-1 arrives.

---

## 3. Timing — when the gain is realized (and when to file)

This is where the IBKR semi-annual rule does NOT apply. Two distinct schemes:

| Scheme | Who it covers | Filing rule |
|---|---|---|
| Semi-annual broker-account scheme | Exchange-traded securities held with a Serbian broker | H1 sales by 30 July; H2 sales by 30 January |
| **Generic individual capital-gains scheme** | Foreign LLC interests, private d.o.o. udeli, real estate, crypto | **Within 30 days** of realizing or starting to realize income from the sale (Article 95 ZPPPA + PPDG-3R uputstvo) |

The Dandilion redemption is in the second bucket.

### When is the gain realized?

The taxable event is **transfer of ownership**, not cash receipt (ZPDG Article 72). Per §3.01 of the Settlement, "the transfer of Redeemed Interest is irrevocable and is to occur upon the Closing Date" — even if installments default later. So:

- **Realization date = Closing Date** (the date you sign + LLC conversion docs are filed in Delaware).
- **Filing deadline = Closing Date + 30 days.**
- **Sale price reported = full £46,000 nominal** (no NPV discounting — Serbia has no installment-method analog to U.S. §453; the agreed contractual price is what gets reported).
- **FX conversion = NBS middle rate on the Closing Date** (one rate, applied to the full £46,000).

### What if installments default later?

If the LLC stops paying (say, after installment 8), you would have already paid 15% on the full £46,000 even though you only received ~£17,600. The remedy is an **izmenjena prijava** (amended PPDG-3R) reducing prodajna cena to amounts actually realized, citing partial non-performance and the §3.41 conditional-release language in the Settlement. Document any default carefully (notices to Company, bank records).

### Alternative position (don't use without advisor sign-off)

Some advisors argue per-installment reporting under "počeo da ostvaruje prihod" (Article 95). This is non-standard and the PU often resists. Use only if a Serbian tax advisor delivers a written memo recommending it.

---

## 4. The cost basis decision — the money question

This is the single biggest variable in your tax bill. ZPDG **Article 74**: "nabavna cena" = the price actually paid to acquire the udeo, increased by CPI from acquisition to transfer.

You paid no cash for the 191 Units in October 2024. They were issued at LLC formation, almost certainly in connection with services (you invoiced the LLC through your PR). There is no Serbian-law appraiser report (procena ovlašćenog procenitelja). There is no gift, no inheritance.

**Three positions, ranked:**

### Position A — Zero (or near-zero) basis [RECOMMENDED — conservative & defensible]

- Report nabavna cena ≈ 0 (or whatever nominal capital-account figure the LLC Agreement assigns to you, if any — pull the Schedule of Members).
- Capital gain ≈ full £46,000 in RSD.
- Tax @ 15% ≈ **£6,900 / ~RSD 970,000** at current FX.
- **Why**: Article 74 stav 1 reads "cena po kojoj je obveznik stekao." No cash paid + no FMV declared as 2024 service income → the price-paid is 0. Practitioner consensus (Trifunović, Luna Star NS, Aktiva Sistem) defaults here when no contemporaneous FMV report exists.
- **Audit risk**: low. PU rarely challenges a taxpayer for self-assessing too aggressively.

### Position B — FMV at vesting becomes basis [requires amended 2024 filings]

- Hire a valuation expert; determine FMV of 21.75% interest in Dandilion LLC on 9 Oct 2024 (likely close to zero — the LLC was newly formed, no revenue, no funding).
- File an **izmenjena 2024 prijava** declaring that FMV as service income (likely "drugi prihodi" under Article 85, taxed at ~16% effective after 20% standardized expenses, or self-employment turnover if argued as PR revenue).
- Pay the 2024 income tax + late-payment interest + potential penalty (5%–10% of tax due).
- Then claim the FMV as basis on the 2026 PPDG-3R.
- **Math**: only worth it if the FMV-step-up benefit (15% × FMV) > (16% × FMV + interest + penalties). Translation: **almost never net-positive** unless FMV at grant was material AND there's a strong audit defense for that FMV.
- **Recommendation**: skip this path unless an advisor models it for your specific numbers and concludes it's net-positive.

### Position C — Aggressive: claim FMV without amending [DO NOT USE]

- Claim a non-zero basis without ever having declared the corresponding 2024 income.
- **Audit-fatal**. The PU's literal reading of Article 74 is "price paid"; if you didn't pay cash and didn't recognize FMV as income, you have no documented basis. This position will not survive an audit.

### Allocation 96/191

Whatever basis you settle on, the **96 redeemed Units carry 96/191 ≈ 50.26% of total basis** (pro-rata). All Units were issued in a single tranche on 9 Oct 2024 → no FIFO question. (Stocks bought across multiple dates use FIFO; same-date issuances are pro-rata.)

### CPI valorization (Article 75)

The basis is automatically grossed up by Serbia's IPC (indeks potrošačkih cena) from acquisition date to transfer date. The PU computes this on PPDG-3R from RZS data; you don't compute it yourself, but verify against [RZS published indices](https://www.stat.gov.rs/sr-Latn/oblasti/cene/potrosacke-cene). For a ~16-month hold (Oct 2024 → Feb 2026), expect ~5–7% cumulative gross-up. Irrelevant if basis is 0.

---

## 5. NBS / Devizno poslovanje — payment routing

The Zakon o deviznom poslovanju (last amended Sl. glasnik RS 19/2025, in force 14 Mar 2025) restricts Serbian residents from holding foreign currency in foreign-bank accounts. Wise/Revolut count as "devize na računu kod banke u inostranstvu" — a regulated activity. Penalties: RSD 5,000–150,000.

**Cleanest plan — instruct the Company to wire installments directly to a Serbian devizni račun:**

1. Open or use existing GBP devizni račun at a major Serbian bank (Banca Intesa, Raiffeisen, Komercijalna, OTP).
2. Send IBAN + SWIFT/BIC to Sally Sfeir at Dandilion.
3. The bank will execute kontrola priliva — provide the Settlement Agreement as the *osnov priliva*. Likely transaction code: **775 / 778** (capital transactions / sale of equity).
4. The bank handles NBS reporting for you.
5. Funds available in GBP (or convert to RSD at your discretion).
6. Keep all SWIFT MT103 confirmations — proof for both PU (capital-gains tax) and NBS.

If you must use Wise/Revolut for transit, move funds to the Serbian bank promptly. Don't park GBP there long-term.

---

## 6. U.S. tax exposure — the §864(c)(8) / §1446(f) wrinkle

You are a Serbian resident, not a U.S. person. There is **no U.S.-Serbia tax treaty**. Two real U.S. tax mechanisms apply:

### §864(c)(8) — TCJA 2017

Gain by a foreign partner on transfer of a U.S. partnership interest is **ECI (effectively connected income) and taxed in the U.S.** to the extent the foreign partner's distributive share of gain on a deemed sale of all partnership assets at FMV would have been ECI. Dandilion is a U.S.-based software company → its goodwill, IP, and operating assets are likely ECI assets → some portion of your gain is U.S.-taxable.

**Action**: request a written **§864(c)(8) Statement** from Dandilion's accountant *before* Closing. This quantifies the U.S. tax bill.

### §1446(f) — 10% gross withholding by the LLC

On a non-PTP redemption, the LLC must withhold **10% of the amount realized** (so ~£4,600 on £46,000) and remit to the IRS, unless you provide a §1446(f) certification. The Settlement's §9.01 "Member responsible for taxes" clause does NOT override this — the LLC is still legally required to withhold or face liability.

**Action**: provide the LLC with:

- Current **Form W-8BEN** (non-U.S. individual). If on file, request a copy and check expiration (renew every 3 years).
- A **§1446(f) Certificate** — the standard route is the §864(c)(8) Statement showing zero/de minimis ECI gain. Alternative: apply to the IRS for a **§1446(f)(4) Withholding Certificate** to reduce withholding (takes weeks).

### File Form 1040-NR for the redemption year

- Report any §864(c)(8) ECI gain.
- Pay U.S. tax at graduated rates on the ECI portion.
- §1446(f) withholding is creditable; refundable if over-withheld.
- **Likely outcome**: small to modest U.S. tax bill, refund or credit if over-withheld via §1446(f).

### Cross-credit against Serbian tax

ZPDG Article 12 allows a unilateral foreign tax credit for taxes actually paid abroad, even without a DTT — capped at the Serbian tax on the same income. Any U.S. tax paid on ECI gain reduces the Serbian tax owed (up to the 15% cap). Document with 1042-S / 8805 / 1040-NR.

### Past K-1 review (2024, 2025)

If the LLC had U.S.-trade-or-business activity, your distributive share of partnership ECI for 2024 and 2025 was U.S.-taxable, and the LLC was supposed to withhold under §1446(a). Verify with Dandilion whether 1446(a) withholding was done on prior-year K-1s. If not, there may be a 1040-NR exposure for those years independent of the redemption.

---

## 7. The retained 95 Units — LLC → Corp conversion

You keep 95 Units that convert to Delaware Corp shares at/near Closing. **This is a separate, unresolved issue** and does NOT affect the redemption filing — but it must be addressed before/at Closing.

- ZPDG **Article 72b** excludes "statusna promena" (status change) where shares/udeli are exchanged exclusively for shares/udeli in the receiving entity per Serbian Companies Law. A Delaware §265 statutory conversion is *analogous* but written for Serbian ZPD entities, so applicability is uncertain.
- **Tax-neutral position** (likely correct): if the Delaware conversion is genuinely a continuity-of-entity event (no liquidation, no recognition under U.S. §351/§368), Serbia respects it — basis carries over, holding period tacks. No PPDG-3R needed.
- **Conservative position**: deemed exchange at FMV → triggers Serbian capital-gains tax on unrealized gain in the 95 retained Units. Expensive.

**Action**: get a **written Serbian tax-advisor opinion** on the conversion *before Closing*. This is a high-leverage deliverable — a bad ruling here could be 2–3× the redemption tax.

---

## 8. Document checklist

Critical (file with PPDG-3R or have ready for PU on demand):

- [ ] Signed Settlement Agreement (with sudski-tumač Serbian translation — NOT optional for PPDG-3R given the foreign-language source document is the basis)
- [ ] LLC Agreement of 9 Oct 2024 with translation, especially the Schedule of Members / Capital Account Schedule
- [ ] Bank confirmation / SWIFT MT103 for first installment received
- [ ] Computation memo: nabavna cena rationale (zero or FMV), CPI valorization (RZS data), prodajna cena (£46,000 × NBS middle rate on Closing day), capital gain, 15% tax

U.S. compliance:

- [ ] Current Form W-8BEN on file with Dandilion
- [ ] §864(c)(8) Statement from Dandilion's accountant
- [ ] §1446(f) Certificate (or evidence the LLC has one)
- [ ] All K-1s issued (2024, 2025, and 2026 partial-year)
- [ ] Forms 1042-S / 8804 / 8805 if any U.S. withholding was done historically
- [ ] Form 1040-NR for the redemption year

Operational / NBS:

- [ ] Serbian devizni račun IBAN + SWIFT communicated to Dandilion
- [ ] Each installment SWIFT confirmation retained
- [ ] Year-end devizni račun statement

Belt-and-suspenders:

- [ ] **Written Serbian tax advisor memo on the LLC→Corp conversion** (95 retained Units, see [§7](#7-the-retained-95-units-llc--corp-conversion))
- [ ] **Written U.S. tax advisor memo on §864(c)(8) ECI quantum**
- [ ] Plan of Conversion / Certificate of Conversion (Delaware filing)
- [ ] Post-conversion Certificate of Incorporation + shareholder agreement
- [ ] 83(b) election copy if filed at original 2024 grant (affects U.S. holding period)

---

## 9. Sequenced action plan

### Before Closing (do NOW — Closing date drives all subsequent deadlines)

1. **Engage advisors** (parallel):
   - Serbian tax advisor: opinion letter on (a) cost-basis position, (b) LLC→Corp conversion treatment for the retained 95 Units, (c) installment-timing approach.
   - U.S. tax advisor: §864(c)(8) ECI analysis + §1446(f) certificate strategy.
2. **Open or confirm Serbian GBP devizni račun**. Send Dandilion the wire instructions before they cut the first installment.
3. **Request from Dandilion**:
   - Current Form W-8BEN copy (renew if >3 years old or expired).
   - §864(c)(8) Statement and §1446(f) Certificate at Closing.
   - All historical K-1s (2024, 2025) and any 1042-S/8805 forms.
   - Schedule of Members / Capital Account Schedule from LLC Agreement.
4. **Sudski tumač translations** of Settlement Agreement and LLC Agreement.
5. **Decide cost-basis position** (Position A recommended). If considering Position B, model with advisor.

### At Closing

6. **Record Closing Date precisely** — this starts the 30-day PPDG-3R clock.
7. **Capture NBS GBP/RSD middle rate** for the Closing Date from [nbs.rs](https://www.nbs.rs).
8. **Compute the gain in RSD** using the chosen basis position.

### Within 30 days of Closing

9. **File PPDG-3R electronically via [ePorezi](https://eporezi.purs.gov.rs)**:
   - Acquisition date: 9 October 2024
   - Acquisition price: per chosen position (RSD)
   - Transfer date: Closing date
   - Sale price: £46,000 × NBS middle rate on Closing date (RSD)
   - Attach: Settlement Agreement, LLC Agreement, computation memo (translations attached).
10. **Wait for the rešenje** (assessment decision from PU). Tax is due **15 days from receipt of the rešenje**.
11. **Pay tax** via the payment instructions in the rešenje.

### Each installment (April 2026 → December 2027)

12. **Retain SWIFT confirmation** for every installment. File in a single folder.
13. **No additional PPDG-3R filings** under Position A (single-realization at Closing).

### Year-end (each year)

14. **2026 income year**: when 2026 K-1 arrives, review for any partnership distributive share of income separate from the redemption — that may require a separate **PP-OPO** filing for foreign income / dividend-equivalent.
15. **File Form 1040-NR** for the redemption year (with U.S. advisor).
16. **Verify CPI/RZS data** matches the PU's valorization computation on the rešenje.

### If LLC defaults on installments later

17. File an **izmenjena PPDG-3R** reducing prodajna cena to amounts actually realized, citing §3.41 of the Settlement (conditional release on Payment Plan compliance).

---

## 10. Open items / risks to escalate to advisors

| # | Risk | Owner | Decision needed before |
|---|---|---|---|
| 1 | Cost basis position (zero vs. FMV-at-grant) | Serbian tax advisor | Closing |
| 2 | LLC→Corp conversion: tax-neutral or deemed exchange? | Serbian tax advisor | Closing |
| 3 | §864(c)(8) ECI quantum + §1446(f) withholding | U.S. tax advisor + Dandilion | Closing |
| 4 | Historical 1446(a) withholding on 2024/2025 K-1s | Dandilion's accountant | Before 1040-NR filing |
| 5 | Per-installment vs. single-realization timing | Serbian tax advisor | First filing |
| 6 | NBS osnov priliva code for installment wires | Serbian bank's compliance | Before first installment |

---

## 11. Illustrative numbers (rough, not for filing)

Assumptions: zero basis (Position A), NBS GBP/RSD ≈ 140 on Closing day.

| Line | Amount |
|---|---|
| Sale price (£46,000 × 140) | RSD 6,440,000 |
| Acquisition price (zero, no cash paid) | RSD 0 |
| CPI valorization | n/a on zero basis |
| Capital gain (RSD) | **RSD 6,440,000** |
| Serbian tax @ 15% | **RSD 966,000 ≈ £6,900** |
| Estimated U.S. tax (§864(c)(8) ECI portion) | $0 to a few thousand USD — needs LLC's analysis |
| Foreign tax credit (Serbia, capped at 15% of same income) | Up to 15% of ECI gain |

Your effective Serbian rate is **15% of nominal £46,000 = £6,900** in the conservative case. Anything paid to the U.S. on ECI portion is creditable in Serbia (subject to cap).

---

## 12. Related notes

- [[ibkr-serbian-tax-guide]] — broader Serbian capital-gains framework, ZPDG article references, 10-year exemption mechanics, NBS rate sourcing, ePorezi mechanics. Foundation reading.

---

## Appendix — Legal references

**Serbian Law on Personal Income Tax (Zakon o porezu na dohodak građana, ZPDG):**

- Article 12 — unilateral foreign tax credit (applies even without DTT).
- Articles 72–80 — kapitalni dobici (capital gains), including foreign udeli.
- Article 72b — 10-year holding exemption + statusna-promena exclusion.
- Article 73 — sale price = contractual or market price.
- Article 74 — acquisition price (cena po kojoj je obveznik stekao); FMV at non-cash contribution at formation.
- Article 75 — automatic CPI valorization of acquisition price.
- Article 85 — drugi prihodi (catch-all for unclassified income).
- Article 87 — annual income tax (godišnji porez); excludes capital gains.
- Article 95 ZPPPA — 30-day filing window from realization or start of realization.

**Serbian Law on Foreign Exchange Operations (Zakon o deviznom poslovanju, ZDP):**

- Article 27 — restrictions on foreign-currency accounts abroad.
- Article 62 — penalties (RSD 5,000–150,000 for individuals).
- Sl. glasnik RS 19/2025, in force 14 March 2025 — most recent amendments.

**U.S. Internal Revenue Code:**

- §864(c)(8) — TCJA 2017 ECI rule on foreign partner gain on partnership-interest transfer.
- §1446(f) — 10% withholding on transferee for non-PTP partnership-interest transfers.
- §1446(a) — withholding on partnership ECI allocations to foreign partners.
- §871, §1441 — non-resident-alien withholding (FDAP, including dividends).
- IRC §351 / §368 — corporate reorganization tax-free treatment (relevant to LLC→Corp conversion).
- 26 CFR §1.1446(f)-2 — final regs on §1446(f) procedures.

**Forms:**

- PPDG-3R — Serbian capital gains, electronic via ePorezi.
- PP-OPO — Serbian self-assessed income (foreign dividends, drugi prihodi).
- W-8BEN — U.S. non-resident-alien individual certification.
- §864(c)(8) Statement — partnership-supplied transferor's certificate.
- §1446(f) Certificate — transferor's certification to reduce/eliminate 10% withholding.
- Form 1040-NR — U.S. non-resident individual tax return.
- Forms 8804 / 8805 — partnership withholding on ECI to foreign partners.
- Form 1042-S — U.S. payor's reporting of FDAP / withholding.

**Treaty status:** No U.S.–Serbia income tax treaty. Article 12 ZPDG unilateral foreign tax credit applies regardless.
