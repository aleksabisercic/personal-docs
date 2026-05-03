---
tags:
  - finance
  - tax
  - serbia
  - capital-gains
  - pausalac
  - dandilion
  - private
category: private
created: 2026-05-01
language: en
summary: Final-signed (4/23/2026) Dandilion settlement — £18k Redemption Price → Aleksa personal capital gain (PPDG-3R, due ~5/23/2026, ~£2,700 tax); £28k Settlement Amount → Lexiconlogic PR consulting revenue (paušalac, KPO knjiga, watch 2027 6m RSD cap).
---

# Dandilion Settlement — Tax Filing Plan

Agreement signed **23 April 2026**. Today is 3 May 2026. **PPDG-3R deadline ≈ 23 May 2026 (~20 days).**

The £46,000 is contractually bifurcated:

| Stream | To | Amount | Tax stream |
|---|---|---|---|
| Redemption Price (§3.03) | Aleksa personal | **£18,000** | Capital gain → PPDG-3R, 15% → ~**£2,700** |
| Settlement Amount (§3.02) | Lexiconlogic PR | **£28,000** | Consulting revenue → paušalac, KPO knjiga, **no incremental income tax** (presumptive base) |

Total Serbian tax on the £46k: **~£2,700**.

The recital ("indivisible package... good-faith characterization") and §3.02 ("consulting fees... due and owing... for services rendered") give bilateral, contemporaneous documentation defending both characterizations.

---

## 1. £18k Redemption Price → PPDG-3R

- **Taxable event**: transfer at Closing (23 Apr 2026; §5.02 makes transfer irrevocable regardless of payments).
- **Filing window**: 30 days from Closing → **deadline 23 May 2026**. Foreign LLC interest sales use the generic 30-day rule, not the IBKR semi-annual scheme.
- **Form**: PPDG-3R via [ePorezi](https://eporezi.purs.gov.rs).
- **Cost basis**: **0**. Units issued for services Oct 2024, no cash paid, no FMV declared as 2024 income. ZPDG Article 74 → "price paid" = 0. Newly-formed LLC on day one had effectively zero FMV anyway. Practitioner default. Higher basis requires amended 2024 filings — almost never net-positive.
- **Sale price**: £18,000 × NBS GBP/RSD middle rate on 23 Apr 2026.
- **Single filing for full nominal £18k** — no NPV discounting, no per-installment reporting.
- **CPI valorization (Article 75)**: PU computes automatically; irrelevant on zero basis.
- **10-year exemption**: not available (held ~18 months).
- **If Dandilion defaults later** (§4.01): file *izmenjena* PPDG-3R reducing prodajna cena to amounts realized.

**Tax**: 15% × £18,000 ≈ **£2,700 / RSD ~378,000**.

### 1.1 PPDG-3R — field by field

Form layout per **Pravilnik 67/2021** (still current in 2026). [Official PDF](https://www.purs.gov.rs/upload/media/2025/2/4/497105/Obrazac-PPDG-3R.pdf) · [PURS uputstvo](https://purs.gov.rs/lat/fizicka-lica/pregled-propisa/uputstva/4579/uputstvo-za-podnosenje-poreske-prijave-za-utvrdjivanje-poreza-na-kapitalne-dobitke-na-obrascu-ppdg--3r.html). Sections 4 (HoV/IF), 5, 6, 7 — leave empty.

**Section 1 — prijava metadata**

| Field | Label | Enter |
|---|---|---|
| 1.1 | Vrsta prijave | `1` (prva prijava) |
| 1.2 | Datum nastanka poreske obaveze | `23.04.2026` |
| 1.3 | Datum dospelosti | leave (PU fills on rešenje) |
| 1.4 | Datum i način podnošenja | filing date + `e` (elektronski) |

**Section 2 — taxpayer**

| Field | Label | Enter |
|---|---|---|
| 2.1 | Tip obveznika | `1` (rezidentno fizičko lice) |
| 2.2 | JMBG | **JMBG**, not the paušalac PIB — file as fizičko lice |
| 2.3 | Ime i prezime | `BISERCIC ALEKSA` |
| 2.4 | Prebivalište | šifra opštine + adresa |
| 2.5 / 2.6 | Telefon / e-mail | personal |

**Section 3 — substantive entry (one row)**

By placing the entry in Section 3 (rather than Section 4 for HoV/IF) you are declaring it as **udeo u kapitalu pravnog lica** under Article 72 ZPDG — there is no separate dropdown.

| Field | Label | Enter |
|---|---|---|
| 3.1 | Redni broj | `1` |
| 3.2 | Datum prenosa | `23.04.2026` |
| 3.3 | Prodajna cena (RSD) | £18,000 × NBS GBP/RSD srednji kurs on 23.04.2026 (single number, no decimals) |
| 3.4 | Datum sticanja | `09.10.2024` |
| 3.5 | Nabavna cena | `0` |
| 3.6 | Kapitalni dobitak | computed: 3.3 − valorized 3.5. With basis 0, equals 3.3. |

**Foreign issuer + zero basis are NOT form fields** — explain both in the **prateći dopis** (cover letter, see §1.2).

CPI valorization (Article 75): enter **raw** nabavna cena. PU computes the index gross-up on the rešenje. Irrelevant on zero basis.

### 1.2 Prateći dopis (cover letter)

PPDG-3R has no field for the foreign issuer or for the basis = 0 rationale. The dopis carries the explanatory weight. Single Serbian-language PDF, signed, attached to the e-prijava. Include:

1. **Transaction**: redemption of 96 Units (50% of holding) of *Dandilion LLC*, Delaware (USA), per Membership Interest Purchase and Settlement Agreement of 23.04.2026. State LLC name, jurisdiction, EIN, Delaware file number, % held pre-redemption.
2. **FX math**: *"Prodajna cena: GBP 18,000 × srednji kurs NBS GBP/RSD na dan 23.04.2026 = X RSD"* — quote the exact NBS rate and attach the kursna lista printout.
3. **Single-realization timing**: *"Iako se kupoprodajna cena isplaćuje u 14 mesečnih rata u periodu maj 2026 – jun 2027, kapitalni dobitak je realizovan u celosti na dan zaključenja Agreement-a, 23.04.2026, te se prijavljuje jednokratno."* (Cite ZPDG čl. 72.)
4. **Basis = 0 rationale**: units issued for services on 09.10.2024 under LLC Agreement; no cash contribution; no FMV deklaracija as 2024 dohodak (LLC was newly formed with no readily ascertainable market value at issuance). Cite **čl. 74 ZPDG** (PU may set nabavna cena at *tržišna vrednost na dan sticanja* if original price not determinable; FMV on 09.10.2024 ≈ 0).
5. **List of attachments**.

### 1.3 ePorezi mechanics

Path: [eporezi.purs.gov.rs](https://eporezi.purs.gov.rs) → login (kvalifikovani elektronski sertifikat — easiest is **ConsentID** mobile app from Office for IT and eGovernment) → switch to **personal JMBG profile** (not the paušalac PIB profile) → *Pojedinačne poreske prijave* → *PPDG-3R* → *Tekstualni unos* → fill Sections 1–3 → *Prilozi* (upload PDFs, ~5 MB each) → *Provera* → *Potpiši* → *Pošalji*.

After submission: GUID identifikacioni broj prijave (your receipt). **Broj predmeta** follows when inspektor opens the file. **Rešenje** lands in your **eSandučić** (eUprava) and as paper to your prebivalište. Foreign-asset cases typically take **30–90 days** for rešenje (vs. ~15 days for domestic). Pay within 15 days of rešenje.

### 1.4 Likely PU follow-ups (pre-empt by attaching everything)

1. *"Dokažite da nabavna cena = 0"* — covered by LLC Agreement + capital account schedule + dopis explanation.
2. *"Dostavite sudski overen prevod ugovora"* — guaranteed if not attached up front. Attach sudski tumač for both contracts.
3. *"Dokažite rezidentnost / nepostojanje stalne poslovne jedinice u Srbiji"* — rare; ignore unless asked.

---

## 2. £28k Settlement Amount → Lexiconlogic PR

Paušalac is taxed on a **presumptive base, not actual revenue** — receiving £28k generates **no incremental income tax**. What it affects:

- **6m RSD annual revenue cap** (paušalac eligibility). Tracked in **KPO knjiga**, cash basis.
- **8m RSD VAT threshold**.
- **Annual GPDG**: paušalac net income (presumptive) feeds into the 3× average-salary aggregation; capital gains do not.

### Year-by-year revenue (cash basis, GBP/RSD ≈ 140)

| Year | Schedule | RSD | Headroom under 6m cap |
|---|---|---|---|
| 2026 (8 mo × £900) | £7,200 | ~1.0m | other PR revenue < ~5.0m |
| **2027** (6×£900 + 6×£2,200) | £18,600 | **~2.6m** | **other PR revenue < ~3.4m** ← tightest |
| 2028 (1 × £2,200) | £2,200 | ~0.3m | other PR revenue < ~5.7m |

**2027 is the cap-pressure year.** Project Lexiconlogic's other 2027 invoicing now.

### Operational

- **Issue one invoice for £28,000** dated ~23 Apr 2026 referencing "outstanding fees per Settlement Agreement". Record each installment receipt against that invoice in KPO knjiga.
- **Wire to Lexiconlogic poslovni devizni račun**, NOT Aleksa's personal IBAN. Co-mingling lets PU recharacterize as Aleksa's drugi prihodi (~16%).
- NBS osnov priliva code: services-rendered (~123).

---

## 3. U.S. exposure (£18k stream only)

- **§864(c)(8)** — portion of the £18k gain allocable to ECI assets is U.S.-taxable. Likely small for a small operating LLC. Need a §864(c)(8) Statement from Dandilion's accountant.
- **§1446(f)** — LLC must withhold 10% × £18k ≈ **£1,800** unless Aleksa furnished a §1446(f) Certificate. §10.01 mutual indemnity does NOT override IRS withholding rules. File **Form 1040-NR** for 2026; §1446(f) is creditable/refundable.
- **Cross-credit** (ZPDG Article 12): U.S. tax paid on ECI gain credits against the Serbian 15% (capped).
- **£28k stream**: services performed in Belgrade by a Serbian PR = foreign-source income (IRC §861) → no U.S. withholding.
- **Past K-1s** (2024, 2025): verify whether 1446(a) was withheld; if not, prior-year 1040-NR exposure.

---

## 4. Retained 95 Units — LLC → Corp conversion (open)

§9.01: 95 retained Units convert to Delaware Corp shares. Independent of the Redemption filing but high-leverage.

- **Tax-neutral** (likely correct) under ZPDG Article 72b "statusna promena" by analogy → no PPDG-3R, basis carries over, holding period tacks.
- **Conservative reading**: deemed exchange at FMV → triggers Serbian tax on unrealized gain in the 95 Units.

→ Get a written Serbian tax-advisor opinion. A bad ruling here costs more than the Redemption Price tax.

---

## 5. Checklist

### Do this week (≤ 10 May)

- [ ] Confirm Closing Date — pull Delaware §265 Certificate of Conversion to verify it filed on/around 23 Apr 2026
- [ ] Verify first installments hit correct accounts (Redemption Price → Aleksa personal; Settlement Amount → Lexiconlogic poslovni)
- [ ] If account routing wrong, contact Sally Sfeir to fix immediately
- [ ] Issue Lexiconlogic invoice for £28,000 dated 23 Apr 2026
- [ ] Capture NBS GBP/RSD middle rate for 23 Apr 2026 (record in computation memo)
- [ ] Engage Serbian tax advisor (cost basis + LLC→Corp conversion opinion)
- [ ] Engage U.S. tax advisor (§864(c)(8) + §1446(f))

### Do week of 11 May

- [ ] Sudski tumač translation: Settlement Agreement
- [ ] Sudski tumač translation: LLC Agreement of 9 Oct 2024 (Schedule of Members in particular)
- [ ] Print NBS GBP/RSD kursna lista for 23.04.2026 ([nbs.rs by date](https://webappcenter.nbs.rs/ExchangeRateWebApp/ExchangeRate/IndexByDate))
- [ ] Compute prodajna cena: £18,000 × that rate
- [ ] Draft **prateći dopis** (cover letter, SR) per §1.2
- [ ] Confirm ConsentID / e-cert is active and JMBG profile works on ePorezi

### Filing-bundle attachments (PDFs for ePorezi)

- [ ] LLC Agreement (EN original + sudski tumač SR)
- [ ] Settlement Agreement (EN original + sudski tumač SR)
- [ ] Capital Account Schedule / Schedule of Members showing $0 contribution
- [ ] NBS kursna lista printout for 23.04.2026
- [ ] Prateći dopis (SR)
- [ ] Bank confirmation of first installment (or expected schedule)
- [ ] Kopija lične karte

### File by 23 May

- [ ] **File PPDG-3R via ePorezi** per §1.1 fields + §1.3 mechanics
- [ ] Save GUID identifikacioni broj prijave (receipt)
- [ ] Pay tax within 15 days of receiving rešenje

### Each installment (May 2026 → Jan 2028)

- [ ] Save SWIFT MT103 confirmation for both streams
- [ ] Update Lexiconlogic KPO knjiga with installment receipt
- [ ] Update 2027 cumulative-revenue tracker (cap pressure year)

### 2026 year-end / early 2027

- [ ] Receive 2026 K-1 from Dandilion; review for partnership distributive share separate from redemption
- [ ] File Form 1040-NR for tax year 2026
- [ ] Verify CPI/RZS valorization on the rešenje (pro-forma since basis is 0)

### If Dandilion defaults

- [ ] Issue Default Notice (§4.02), wait 10 business days for cure
- [ ] Accelerate per §4.03 if uncured
- [ ] File *izmenjena* PPDG-3R reducing prodajna cena to amounts realized; revise KPO knjiga

---

## 6. Key dates

| Date | Event |
|---|---|
| 23 Apr 2026 | Closing / agreement signed |
| ~early May 2026 | First installments due (within 7 BD of execution) |
| **23 May 2026** | **PPDG-3R deadline** |
| 1st BD of each month | Subsequent installments |
| Jul 2027 | Settlement Amount installments step up from £900 to £2,200 |
| Jun 2027 | Last Redemption Price installment (£1,100) |
| Jan 2028 | Last Settlement Amount installment |
| Mar–Apr 2027 | 2026 K-1 expected |
| Apr 2027 | File Form 1040-NR for 2026 |
| 15 May 2027 | PP GPDG deadline (if applicable) |

---

## 7. Open questions for advisor

1. Cost basis = 0 confirmed?
2. LLC→Corp conversion: tax-neutral or deemed exchange for the 95 retained Units?
3. §864(c)(8) ECI quantum on the £18k?
4. Any 1446(a) withholding done on 2024/2025 K-1s?
5. Per-installment vs. single-realization PPDG-3R timing — confirm single-realization is the right call?

---

## Related

- [[ibkr-serbian-tax-guide]] — Serbian capital-gains framework, ZPDG references, NBS rates, ePorezi mechanics.
