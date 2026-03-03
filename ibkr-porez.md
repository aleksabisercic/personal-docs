# Serbian Tax Guide for US Stock Investments via Interactive Brokers

**A Serbian tax resident holding US stocks through Interactive Brokers owes 15% on capital gains and 15% on dividends — but the absence of a US-Serbia tax treaty means 30% US withholding on dividends, half of which is effectively lost.** This creates a total dividend tax burden of 30% (all paid to the US, with Serbia zeroed out by credit) and a straightforward 15% on capital gains (untaxed by the US). Capital gains are filed semi-annually on form PPDG-3R; dividends are filed within 30 days of receipt on form PP-OPO. The single most powerful optimization available is the **10-year holding exemption** — securities held for a decade are completely tax-free on sale (you still file, but tax is 0%). This guide covers every obligation, form, deadline, and Interactive Brokers report needed to stay compliant, based on the Zakon o porezu na dohodak građana (Law on Personal Income Tax) as amended through early 2026.

---

## Filing when trading through IBKR

When trading via Interactive Brokers, you submit **trade confirmations** for both purchases and sales. These must show your **name, date, and address**. You can set up a custom template in IB to include exactly the data you need. There is **absolutely no need for court-certified translation** ("sudski tumač") — the documents contain minimal text (mostly numbers, dates, and names), so translation is unnecessary. Just make sure all required information is visible.

---

## The 15% capital gains tax and how to file it

Serbia taxes capital gains from selling securities at a **flat 15% rate** under Article 77 of the Zakon o porezu na dohodak građana (ZPDG). The taxable base is the difference between the sale price and acquisition price, both converted to Serbian dinars. The US does not tax non-resident aliens on portfolio capital gains, so only Serbia collects here.

**Filing is semi-annual, not per-transaction.** All stock sales from January 1 through June 30 are reported on a single PPDG-3R form due by **July 30** of the same year. Sales from July 1 through December 31 are reported on a second PPDG-3R due by **January 30** of the following year. After you file, the Poreska Uprava (Tax Administration) reviews your submission and issues a formal assessment decision ("rešenje"). You have **15 days** from receiving that decision to pay.

### Cost basis — FIFO and separate filings per lot

Cost basis follows a **chronological/FIFO matching** approach. You must match sales to the **oldest purchase lots first**. Critically, if you bought shares on different dates and sell them all at once, **you must file a separate entry for each purchase lot**.

**Example:** You buy 10 shares on January 1, 2025, then buy 20 more shares on January 2, 2025, then sell all 30 shares on January 3, 2025. You must create **two separate filings**:
1. "Bought 10 shares on Jan 1, sold those 10 on Jan 3"
2. "Bought 20 shares on Jan 2, sold those 20 on Jan 3"

The reason: you cannot cherry-pick which lot you're selling. The oldest shares must be sold first. This is directly tied to the **10-year holding exemption** — you cannot claim to sell only your newest shares while holding old shares to reach the 10-year tax-free threshold.

### Currency conversion

We buy in euros or dollars, but currencies fluctuate — **everything must be reported in dinars**. It is possible to have a nominal gain in foreign currency but, due to exchange rate movements, actually break even or have a loss in RSD terms.

**Currency conversion uses the NBS middle exchange rate on each transaction date.** The purchase price converts at the NBS middle rate on the date you bought the shares; the sale price converts at the rate on the sale date. This creates an FX component in your gain or loss that is embedded in the calculation — you do not report FX gains separately. All amounts on PPDG-3R are entered in RSD. The NBS publishes daily middle rates at nbs.rs.

### Inflation adjustment — the tax office handles it

The acquisition price is **increased by Serbia's annual inflation rate** (indeks potrošačkih cena). This is a significant benefit.

**Example:** You buy shares for 1,000 EUR. You sell them a year later for 2,000 EUR. Your gain is 1,000 EUR. But if inflation in Serbia was 10% that year, your acquisition price is increased by 10% — as if you bought for 1,100 EUR. So your taxable gain is only 900 EUR, meaning less tax.

**You do not need to calculate this yourself.** The Poreska Uprava (Tax Administration) applies the inflation adjustment automatically when they process your filing and issue the rešenje (assessment decision).

### Capital loss carry-forward

**Capital losses can offset future gains for 5 years** under Article 78. You **must** file the PPDG-3R even when realizing a loss — this is not optional. The tax authority issues a rešenje confirming the loss amount, which you reference when offsetting against future gains. Losses cannot offset other income types (salary, self-employment, etc.) and cannot be carried back.

You can also strategically realize losses — for example, selling a position at a loss and immediately buying a similar fund — to bank a capital loss for tax purposes.

**Worked example:** You buy 10 shares of GOOG on March 15, 2025 for $5,000 USD when the NBS middle rate is 109.50 RSD/USD. Your RSD cost basis is 547,500 RSD. You sell on October 20, 2025 for $7,000 USD when the NBS rate is 110.20 RSD/USD. Your RSD proceeds are 771,400 RSD. Capital gain = **223,900 RSD**. Tax at 15% = **33,585 RSD** (approximately $305). You report this on the PPDG-3R for the second half of 2025, due January 30, 2026.

---

## The 10-year holding exemption

Under Article 72a(1)(5) of the ZPDG, securities held continuously for **over 10 years** are **completely exempt from capital gains tax**. You still file the PPDG-3R, but the tax is **0%**.

For a long-term investor building a substantial portfolio, this turns a 15% lifetime tax bill into zero. This single provision should drive portfolio strategy: buy quality, hold indefinitely, and avoid selling before the decade mark unless losses need harvesting.

This is also the reason FIFO lot matching and separate lot filings matter — you cannot game the system by claiming to sell newer shares while holding older ones to reach the 10-year mark.

---

## Dividends face a painful 30% US withholding with no treaty relief

This is where the absence of a US-Serbia Double Taxation Treaty causes real financial pain. **No DTT has ever existed between the US and Serbia** — confirmed by the IRS treaty list, US Treasury records, and KPMG Serbia's roster of Serbia's 64 treaty partners. The US and Yugoslavia never signed one either. Negotiations between the US and Serbia are ongoing but no timeline for conclusion exists.

Without a treaty, the **US withholds 30% on dividends** paid to Serbian residents. Filing Form W-8BEN with Interactive Brokers does not reduce this rate — its purpose is to certify your non-US status (preventing even worse backup withholding on sale proceeds) rather than claiming a treaty rate. The W-8BEN is still essential: without it, IB may apply **24% backup withholding on gross sale proceeds** in addition to dividend withholding.

**Serbia taxes dividends at 15%** as "prihodi od kapitala" (income from capital) under Articles 61–65 of the ZPDG. However, Article 12 provides a **unilateral foreign tax credit** ("poreski kredit"): if you paid tax on income in another country, you receive a credit against Serbian tax, capped at the Serbian tax amount on that income. This applies even without a DTT.

**The math on a $1,000 US dividend:**

| Step | Amount |
|------|--------|
| Gross dividend received | $1,000 |
| US withholding at 30% | −$300 (paid to IRS) |
| Net received in IB account | $700 |
| Serbian tax at 15% on gross $1,000 | $150 |
| Foreign tax credit (capped at Serbian tax) | −$150 |
| **Net Serbian tax owed** | **$0** |
| **Total tax paid** | **$300 (all to US)** |
| **Effective rate** | **30%** |
| **Excess US tax — unrecoverable** | **$150** |

You owe nothing additional to Serbia, but **$150 per $1,000 in dividends is permanently lost** to the excess US withholding. This makes US dividend-paying stocks significantly less tax-efficient for Serbian residents. Filing is done on form **PP-OPO** within **30 days** of receiving each dividend, using income code **1 11 402 00**. PP-OPO is self-assessment: the system generates payment instructions immediately upon submission, and the tax (if any after credit) is due within the same 30-day window. Each dividend payment requires a separate PP-OPO filing.

One area of practitioner debate exists: while the prevailing professional interpretation holds that Article 12's unilateral credit applies regardless of whether a DTT exists, some tax inspectors have been inconsistent. **Retain your IB Form 1042-S** as proof of US tax paid — this is the key document for claiming the credit.

---

## Reporting obligations, foreign accounts, and the NBS question

**There is no Serbian equivalent of the US FBAR.** Serbia does not require individuals to file a standalone annual declaration of foreign financial assets with the tax administration. If you hold stocks but make no sales and receive no dividends in a given period, you have **no tax filing obligation** for that period.

However, a separate obligation exists under the **Zakon o deviznom poslovanju** (Law on Foreign Exchange Operations). Article 27 technically requires Serbian residents to obtain **prior NBS (National Bank of Serbia) approval** to hold foreign currency at foreign institutions. After collecting sale proceeds, the resident is theoretically required to **repatriate funds to a domestic account within 30 days**.

**In practice, enforcement of NBS rules on retail investors has been minimal.** Thousands of Serbian residents use Interactive Brokers without NBS approval, and no public cases of enforcement against retail investors have emerged. Nevertheless, the legal obligation exists, and penalties for violations range from **RSD 100,000 to 2,000,000** (approximately €850 to €17,000).

For the **annual income tax** (godišnji porez na dohodak građana, form PP GPDG): if your total qualifying net income exceeds **3× the average annual salary** (RSD 4,874,508 for 2024, approximately €41,500), you must file by **May 15** of the following year. Capital gains are **excluded** from this calculation, but dividends are included. The PP GPDG is filed exclusively electronically via the ePorezi portal.

**Paušalac interaction:** Personal stock trading creates no conflict with your paušalac (lump-sum taxed sole proprietorship) status. Capital gains and dividends from personal investments are filed separately as an individual, not through the business.

---

## How to map Interactive Brokers reports to Serbian tax forms

Interactive Brokers provides several reports for non-US persons, all denominated in **USD** (IB does not offer RSD-denominated reports). You must manually convert every figure to RSD using the NBS middle rate.

You submit **trade confirmations** for purchases and sales. Make sure they show your **name, date, and address**. You can set up a custom template in IB. There is no need for translation — the documents are mostly numbers and minimal text.

| Tax obligation | IB report to use | Key fields/columns | Serbian form + field | Conversion note |
|---|---|---|---|---|
| Capital gains (realized P&L) | **Activity Statement → Trades section** | Date, Symbol, Quantity, Price, Proceeds, Cost Basis, Realized P&L (FIFO), Comm/Tax | **PPDG-3R** — purchase price, sale price, gain/loss per security | Convert purchase price at NBS rate on buy date; sale price at NBS rate on sell date |
| Cost basis by lot | **Activity Statement → Open Positions section** | Cost Basis, Date Acquired, Quantity | PPDG-3R — acquisition price fields | NBS middle rate on original purchase date |
| Dividends received | **Activity Statement → Dividends section** or **Year-End Dividend Report** | Date, Description, Amount | **PP-OPO** — gross income field, code 1 11 402 00 | NBS middle rate on dividend payment date |
| US withholding tax paid | **Activity Statement → Withholding Tax section** or **Form 1042-S** (Box 7) | Date, Amount withheld, Rate | PP-OPO — foreign tax credit (poreski kredit) field | Same conversion date as dividend |

**To download these reports:** Log into Client Portal at portal.interactivebrokers.com → **Performance & Reports** → **Statements** → **Activity** tab. Select the "Legacy Full" template, choose "Annual" or a custom date range covering the semi-annual period (Jan–Jun or Jul–Dec), and download in CSV format for Excel processing. For the 1042-S: **Performance & Reports** → **Tax Documents** → **Tax Forms** (available by March 15 following the tax year).

**Cost basis method:** IB's default cost basis method is **FIFO**, which aligns with Serbian practice. However, IB may apply US wash sale adjustments on some reports — Serbian law has no wash sale rules, so if you see "wash sale loss disallowed" entries, you may need to manually reverse these when filing in Serbia.

### Filing fractional shares — ePorezi limitation

If you sold a **fractional number of shares** (e.g., 1.2 shares) during a semi-annual period, the ePorezi online portal **cannot handle decimal quantities**. The website silently replaces decimal numbers with 0 — neither "." nor "," works as a decimal separator. This has been confirmed by calling the tax administration in Belgrade.

**Workaround:** Download the PPDG-3R form in **PDF format** (it has the same fields and field numbers as the online version). Fill it out manually in the PDF, print it, and submit it **in person** at your local Poreska Uprava office. The clerk will accept the paper form and give you a receipt with a case number ("broj predmeta").

### Filing electronically

Both PPDG-3R and PP-OPO can be filed through the **ePorezi portal** (eporezi.purs.gov.rs) using a qualified electronic certificate (loaded on your national ID card or via ConsentID cloud signature). You enter transaction data manually — there is no import function from IB. For the PPDG-3R, attach your IB Activity Statement as supporting documentation.

---

## Optimization strategies and compliance risks to manage

**The 10-year holding exemption is the most powerful tool available.** Securities held continuously for over 10 years are **completely exempt from capital gains tax** (you still file, tax is 0%). For a long-term investor building a $100,000+ portfolio, this turns a 15% lifetime tax bill into zero.

**Tax loss harvesting is explicitly valuable.** Since losses carry forward for 5 years, deliberately realizing losses on declining positions before each semi-annual cutoff (June 30 and December 31) creates tax assets. You can sell at a loss and immediately buy a similar fund to maintain market exposure while banking the loss. However, you must file the PPDG-3R documenting the loss to establish the carry-forward — unfiled losses are wasted.

**Restructure away from US-listed dividend stocks.** The 30% US withholding with only 15% creditable makes US dividend payers highly tax-inefficient. Two better alternatives exist:

- **Ireland-domiciled accumulating ETFs** (e.g., CSPX, VWRA on London Stock Exchange): Ireland has a 15% US dividend treaty rate, and Serbia has a DTT with Ireland. Accumulating funds reinvest dividends internally, avoiding the Serbian 30-day filing obligation entirely.
- **Non-dividend growth stocks** (like GOOG, AMZN, MSFT): These pay minimal or no dividends, making the treaty absence largely irrelevant. Capital gains face only Serbia's 15% with no US tax.

**Common mistakes to avoid:**
- Not filing on losses (losing the 5-year carry-forward)
- Using the wrong exchange rate (must be NBS middle rate, not your bank's commercial rate)
- Missing the 30-day dividend filing window
- Not renewing the W-8BEN every 3 years with IB (expiration triggers backup withholding on proceeds)
- Forgetting that each dividend payment requires a separate PP-OPO filing
- Trying to file fractional shares online (use the PDF form instead)

**Penalties for non-compliance** range from administrative fines of **RSD 5,000 to 150,000** (€42–€1,280) for late or missed filings, plus **late payment interest** at the NBS reference rate + 10 percentage points per annum. For deliberate tax evasion exceeding RSD 1,000,000 (€8,500), criminal penalties apply.

**Do you need a tax advisor?** For a portfolio of $20,000 with occasional trades, self-filing through ePorezi is straightforward once you've done it once. Don't panic about the process — it is not as complicated as people make it seem, and there is no need to pay a local broker extra fees for Serbian-language reports.

---

## Step-by-step compliance checklist

**After each stock sale (within the semi-annual period):**

1. Record the trade date, number of shares, sale price in USD from IB's Trades section of the Activity Statement.
2. Identify the matching purchase lot(s) using FIFO — oldest shares sold first. Make separate entries per lot.
3. Look up the NBS middle exchange rate for both the original purchase date and the sale date at nbs.rs.
4. Convert the purchase price and sale price to RSD separately. Calculate the gain or loss in RSD.
5. Before the semi-annual deadline (July 30 or January 30), log into ePorezi, file PPDG-3R with all transactions for that half-year, and attach IB's Activity Statement (trade confirmations showing name, date, address).
6. The inflation adjustment to your acquisition price will be applied automatically by the tax office — you do not need to calculate it.
7. Wait for the Poreska Uprava to issue a rešenje (assessment). Pay within 15 days of receiving it.

**After each dividend receipt:**

1. Note the payment date and gross dividend amount from IB's Dividends section.
2. Note the US withholding tax from IB's Withholding Tax section (or Form 1042-S at year-end).
3. Convert the gross dividend to RSD using the NBS middle rate on the payment date.
4. Within 30 days, file PP-OPO on ePorezi with income code 1 11 402 00, claim the foreign tax credit for US tax paid (capped at 15% of gross dividend in RSD), and pay any remaining tax immediately.

**Documents to retain:** IB Annual Activity Statement (Legacy Full, CSV and PDF), Form 1042-S, Year-End Dividend Report, NBS exchange rate records for each transaction date, all filed PPDG-3R and PP-OPO forms with confirmation receipts, and all rešenje decisions received from the tax authority. Serbian tax records should be kept for at least **5 years** (the statute of limitations for tax assessment).

---

## Appendix: legal references and key provisions

**Serbian Law on Personal Income Tax (Zakon o porezu na dohodak građana):** Article 12 (unilateral foreign tax credit), Articles 61–65 (income from capital/dividends), Articles 72–80 (capital gains), Article 72a(1)(5) (10-year exemption), Article 74 (acquisition price definition), Article 75 (inflation indexing of acquisition price), Article 77 (15% tax rate), Article 78 (loss carry-forward), Article 95 (filing deadlines).

**Serbian Law on Foreign Exchange Operations (Zakon o deviznom poslovanju):** Article 27 (foreign accounts), Article 62 (penalties).

**US-Serbia Double Taxation Treaty:** Does not exist. No predecessor US-Yugoslavia treaty existed. Negotiations are ongoing with no announced timeline.

**US tax treatment of non-resident aliens:** IRC §871 (capital gains exemption for NRAs present fewer than 183 days), IRC §1441 (30% withholding on FDAP income including dividends for non-treaty countries).

**Serbian tax forms:** PPDG-3R (capital gains, semi-annual), PP-OPO (self-assessed income including dividends, per receipt), PP GPDG (annual income tax, if threshold exceeded).

**Filing portal:** ePorezi — eporezi.purs.gov.rs (requires qualified electronic certificate).

**NBS exchange rates:** Available daily at nbs.rs under "Kursna lista."

**IB reports location:** Client Portal → Performance & Reports → Statements (Activity Statements), Tax Documents (1042-S, Dividend Report, Tax Optimizer).

**Key uncertainties flagged:** The applicability of Article 12's unilateral foreign tax credit without a DTT is the prevailing professional interpretation but has seen inconsistent treatment by some tax inspectors. For portfolios generating significant dividend income, retain Form 1042-S as proof. NBS foreign account regulations are technically binding but enforcement against retail investors has been minimal — this may change as Serbia moves toward EU accession and full CRS implementation.
