# Handoff brief: Sunshine Group vs Vingroup, KRW land-secured bond

Audience: the agent/analyst taking this over. Goal: turn a first-pass research pack into a professional, presentation-grade deliverable for senior management.

## 1. Context
- Client: Sunshine Group JSC (HNX: KSF), Hanoi real-estate group. Not "Sun Group" (sungroup.com.vn) - that is a different company; ignore any earlier mention.
- Plan: issue a KRW bond in Korea (Arirang bond), secured by land in the Ciputra urban area (Nam Thang Long), Hanoi.
- Benchmark: Vingroup's debut KRW bond (Korea's first Vietnamese corporate Arirang bond, expected pricing mid-October 2026).
- The boss's instruction was only "research and compare the financials of the two companies and analyse what is needed". No specific question was given, so the open question is part of your job (see section 5).

## 2. What has been done (first pass = information gathering)
Files are on branch `claude/upbeat-goodall-xqbcly` under `output/` (draft PR #1 in vnvitalii-web/App-bank):
- `Sunshine_vs_Vingroup_Credit_Model.xlsx`: sheets README, Data (inputs), Ratios (formulas), Collateral (LTV calculator, placeholder inputs), Flags (diligence points).
- `Memo_Sunshine_vs_Vingroup.docx`: ~2-page memo.
- `Slides_Sunshine_vs_Vingroup.pptx`: 10 plain slides (not professionally designed).
Source PDFs (uploaded by the user to `main`, public repo; to be deleted): Vingroup Annual Report 2025 (EY audited), Sunshine Group Annual Report 2025 (Deloitte audited; financial statements are SCANNED IMAGES, read visually).

## 3. Key findings so far (FY2025, VND bn)
| | Vingroup | Sunshine |
|---|---|---|
| Total assets | 1,118,623 | 120,144 (was 20,558; +484%) |
| Net revenue | 331,838 | 20,198 (was 2,469) |
| Profit after tax | 11,065 | 8,906 |
| Borrowings | 338,501 | 23,623 (was 946) |
| Equity | 151,489 | 19,863 |
| Borrowings/equity | 2.2x | 1.2x |
| Net debt/EBITDA | 3.0x | 1.6x |
| EBITDA/interest | 3.0x | 18.1x |
| Current ratio | 1.12x | 1.54x |

Narrative: Sunshine is ~11% of Vingroup by assets, 6% by revenue. Headline ratios favour Sunshine, but the year is exceptional (6x asset growth, 95% of revenue from real-estate handovers, short-term receivables VND 57.7tn = 48% of assets, Deloitte emphasis-of-matter on extended loan/cooperation-contract terms, operating cash flow inflated by customer deposits). Collateral helps recovery, not earnings quality.

Vingroup Korean bond (press only, not yet issued): board resolution 11 Aug 2026, up to KRW 455bn, deal ~KRW 300-400bn, 3 years, fixed coupon capped at 8% (Korean press expects ~7%), private placement to Korean institutions, Shinhan Securities Vietnam sole arranger plus KB and Kiwoom, Shinhan invests KRW 40bn, ~KRW 300bn demand secured, use of proceeds general corporate. Reported as SECURED by 4 outlets (MarketScreener, Investing.com, Nguoi Quan Sat, StockBiz); CafeF says unsecured; pledged assets undisclosed. A Gate.com article saying "KRW 4,000 billion" is a mistranslation of 4000억 (= KRW 400bn).

## 4. Known weaknesses / do not trust blindly
- Sunshine numbers were read from low-resolution scans: re-verify every input in the Data sheet against the original audited statements, and read Notes 10, 11, 13, 19, 27, 28 and the acquisition/consolidation notes in full (not yet done).
- The VND 5.8tn HDBank loan secured on the Sunshine Crystal Tay Ho project (Nam Thang Long/Ciputra) was read from a rotated scan: verify. It implies the Ciputra land may already be pledged.
- EBITDA is analyst-defined (PBT + interest + D&A); interest may exclude capitalised interest; net debt uses cash only.
- Vingroup figures come from the annual report MD&A and notes; Vingroup EBITDA includes large non-operating "other profit" (shown also as Adj. EBITDA).
- Collateral sheet inputs are PLACEHOLDERS: land value VND 10tn, haircut 30%, target LTV 60%, FX 18 VND/KRW, bond KRW 400bn. With these the land needs ~VND 17.1tn appraised value.
- Vingroup's bond security terms and pricing are from press, not from the offering memorandum or the original board resolution (check vingroup.net / HOSE).
- The KED article that started the task could not be opened (site blocked). No market pricing/peer comparison exists yet. Several sites (kedglobal, sungroup.com.vn, vietnambiz, theinvestor) were blocked in the first environment; check what you can access.
- Slide deck was not visually rendered/checked.

## 5. Your tasks
1. Clarify the objective with the project owner (user: vnvitalii@gmail.com) in one line: is the question (a) can Sunshine issue and at what price, (b) how much collateral is needed, (c) overall credit story vs Vingroup? Default to (c) with (a)/(b) as conclusions.
2. Verify and complete the data: re-key Sunshine statements from the originals (use a text version if obtainable), add FY2023 if available, add H1 2026 for both (Vingroup H1 2026 revenue VND 222.3tn, PAT VND 20.4tn per press), add debt maturity profile and currency split for both, receivables breakdown for Sunshine.
3. Add comparables: other Vietnamese/foreign issuers of Arirang or KRW bonds, rating-agency views on Vingroup and Vietnamese developers, Korean market spreads. Estimate indicative pricing range for Sunshine vs Vingroup's ~7% with reasoning.
4. Build a proper collateral analysis once documents exist: land-use certificates, mortgage registry extract, existing bank liens and release plan, independent valuation, enforceability for foreign bondholders (security agent, Vietnamese law), FX hedging cost, withholding tax, approvals for foreign borrowing.
5. Produce the final deliverables, professionally designed:
   - Investment-committee style deck (12-15 slides): executive summary with a clear recommendation; peer snapshot; financial comparison charts (leverage, coverage, growth, margins); quality-of-earnings and balance-sheet risks; Vingroup bond benchmark; collateral/LTV analysis with sensitivity; proposed structure and covenants; risks and mitigants; next steps and timeline. Consistent template, titles that state the conclusion, sources on every slide.
   - Formatted Excel model: clean layout, named inputs, charts, scenario/sensitivity, no hard-coded numbers in formulas, source column for every input, check cells.
   - 3-5 page memo with executive summary, same conclusions as the deck.
6. QA: reconcile every number between model, memo and deck; label estimates and unverified items clearly; list open items.

## 6. Quality standards
- Never invent figures. Every number needs a source (document + page) or is labelled ASSUMPTION / UNVERIFIED.
- Keep units explicit (VND bn, KRW bn) and FX assumptions visible.
- Neutral, factual tone; flag disagreements between sources instead of choosing silently.
- Treat client material as confidential: do not push client documents or analysis to a public repo; the repo vnvitalii-web/App-bank is PUBLIC.

## 7. Open items needing the client / project owner
- Land documents for the Ciputra plots and a valuation.
- Target bond size, tenor, timing and use of proceeds.
- Sunshine's own audited originals (not scans) and management accounts for 2026.
- Confirmation of which Sunshine entity would issue and which entity owns the land.
