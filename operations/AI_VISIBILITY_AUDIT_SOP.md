# Tony Intelligence — AI Visibility Audit Operations SOP

Status: Canonical V1 operating procedure
Owner: Reece
Product: AI Visibility Audit
Price: $49 one-time
Intake: https://tonyintelligence.com/audit-intake/
Support: reece@tonyintelligence.com

## 1. Paid order and intake reconciliation

Reece owns the fulfillment queue unless explicitly reassigned.

The manual source of truth is:
Stripe paid order + email intake (legacy Tally submissions may also be reconciled).

An audit enters fulfillment only when both are present and reasonably reconciled.

### Paid order + matching intake
- Confirm Stripe shows a paid, live, $49 AI Visibility Audit order.
- Match by customer email and business identity.
- Record fulfillment start and deadline.
- Proceed.

### Paid order + no intake
- Do not start the 24-hour clock.
- Send a manual reminder with the canonical intake URL.
- Keep the order open until usable intake arrives.

### Intake + no obvious paid order
- Do not begin fulfillment.
- Check Stripe using the submitted email, business identity, and nearby purchase time.
- If no match is found, ask the customer for the email used at checkout or the Stripe receipt/session reference.
- Escalate unresolved identity to Reece.

### Different Stripe and intake emails
- Reconcile using business name, website, purchase time, customer name, and customer confirmation.
- If still ambiguous, ask which email was used at checkout.
- Record both emails once matched.

### Duplicate intake
- Treat submissions for the same paid order as one job.
- Use the newest complete submission unless the customer clearly says otherwise.
- Preserve earlier submissions as reference.

### Customer says they paid but intake cannot be found
- Verify payment in Stripe first.
- If confirmed, resend the canonical intake link and request submission/resubmission.
- If payment cannot be confirmed, request only the minimum order identifiers needed to locate it.
- Do not infer payment.

## 2. 24-hour control

The 24-hour fulfillment clock starts only when:
1. Stripe payment is confirmed paid for the canonical $49 audit.
2. A usable intake is received and reconciled.

Record:
- paid timestamp
- intake timestamp
- fulfillment-start timestamp
- deadline = fulfillment-start + 24 hours

If intake is incomplete, request the missing non-sensitive information. The clock starts when intake becomes usable.

## 3. Fulfillment checklist

- [ ] Paid order confirmed
- [ ] Intake confirmed and reconciled
- [ ] Fulfillment start recorded
- [ ] 24-hour deadline recorded
- [ ] Business identity established
- [ ] Research started
- [ ] Evidence captured
- [ ] Findings classified
- [ ] Report drafted
- [ ] QA completed
- [ ] PDF rendered and visually checked
- [ ] Report delivered
- [ ] Completion recorded

## 4. Evidence standard

Use official business sources first where available.
Use corroborating public sources when useful.
Every material finding must be tied to evidence.

For each finding preserve:
- observed fact
- source name
- source URL
- date checked
- proof or screenshot when useful
- classification
- interpretation
- recommendation

Classify as:
- Observed fact
- Corroborated fact
- AI/search observation
- Interpretation
- Uncertain

Rules:
- Separate observed fact from interpretation.
- Label uncertainty clearly.
- Never invent AI/search visibility claims.
- Never generalize a dated observation into a permanent claim.
- Never claim a fix guarantees rankings, recommendations, traffic, leads, or revenue.
- Treat AI output as an object being audited, not authoritative business truth.

## 5. Report standard

Use:
1. Executive snapshot
2. Strengths
3. Verified gaps/issues
4. Fact vs interpretation separation
5. Evidence/sources
6. Do Now
7. Do Next
8. Later
9. Three practical next actions
10. Limitations/uncertainty

Required:
- business name
- relevant location
- audit date
- supporting sources
- plain-English wording

Do not use:
- fake visibility scores
- invented percentages
- guaranteed ranking claims
- guaranteed AI recommendation claims
- unsupported causal claims

## 6. QA checklist

Before delivery verify:
- [ ] Correct customer and business
- [ ] Correct website/location identity
- [ ] Every material claim has evidence
- [ ] Source URLs support the claim
- [ ] No unsupported claim
- [ ] No unresolved contradictory identity detail
- [ ] Fact separated from interpretation
- [ ] Uncertainty labeled
- [ ] Recommendations specific and actionable
- [ ] No unnecessary private information
- [ ] No permanent claim from a dated AI/search observation
- [ ] No ranking/recommendation guarantee
- [ ] PDF renders cleanly
- [ ] No clipping or overflow
- [ ] Customer can identify the three next actions

A report that fails QA does not ship.

## 7. Delivery procedure

File name:
Tony-Intelligence-AI-Visibility-Audit-[Business-Name]-YYYY-MM-DD.pdf

Send the final PDF to the reconciled customer email.

Delivery message includes:
- audit is complete
- attached report
- findings are a dated public-information snapshot
- customer may reply with questions
- support: reece@tonyintelligence.com

After sending, record:
- customer/business
- Stripe payment identifier
- intake identifier or submission timestamp
- fulfillment start
- deadline
- delivery timestamp
- delivery email
- report filename
- status COMPLETE

If delivery fails:
- verify the reconciled customer email
- use another already-verified customer email only if clearly tied to the same order
- record the failure and retry

If the customer reports a missing attachment:
- verify the existing order/intake context
- resend the same approved report
- regenerate only when an actual correction is required

## 8. V1 operating principle

Manual is acceptable when documented and reliable.

Do not automate research judgment, severity, recommendations, final QA, or delivery merely for convenience.

Canonical flow:
confirmed payment -> confirmed intake -> evidence-backed research -> human judgment -> QA -> professional delivery

## 9. Founding-audit scope and research protocol (2026-10-16 update)

The live commercial scope is https://tonyintelligence.com/audit/. Preserve the $49 price and 24-hour promise. One business, one domain, one primary location/service area; up to five key pages. No fixed minimum finding count: give up to three useful actions and explicitly say when fewer are warranted. The older 'three next actions' checklist must not cause invented findings.

Research sequence (target 45-60 minutes, measure actual time):
1. 0-5 min: reconcile the live paid order and usable intake. Price is USD 49 subtotal, quantity one, canonical product prod_V5ocUB6MeefBA2 / price_1U5cz9KuXqFoa4mbKnLLX0Cg. Total may exceed $49 due to tax. Confirm paid, not merely complete/open, and check refund status before fulfillment. Duplicate intake does not create another job. Record identifiers privately, never in this public repository.
2. 5-15 min: establish identity from official homepage, about, contact, primary service and booking page. Record exact URL, accessed UTC time, excerpt and retrieval method. Compare name, service area, hours and public contact details. A difference between registered address and service area is not automatically an error. Do not publish residential addresses in reports.
3. 15-25 min: inspect public listing/review sources and branded search. Queries: exact business + city; domain; service + city. Record engine/tool, wording, result context, and date. Search snippets are discovery evidence only; open the supporting page before making a material finding. Website testimonials are not independently verified reviews.
4. 25-35 min: check HTTPS, public page status, contact/booking links without submitting, robots, sitemap and index directives. Extract structured data when present and compare to visible text. Do not run intrusive scans, login attempts, port scans, or send test leads. A fetch failure or bot block is 'unable to verify', not proof the customer's site is broken. Do not mark ordinary absent headers as a security incident.
5. Optional within this window: test actual AI answer surfaces only if available without new paid tools. Record exact prompt, model/surface, search on/off, time, sources and full answer privately. Separate branded questions from unbranded category questions. Repeat a prompt when practical; no universal visibility score. If unavailable say 'not tested'. Web search is NOT a ChatGPT/Gemini/Perplexity test. Don't substitute model recollection or invent an answer. No mandatory llms.txt, special AI markup, or keyword hacks; Google's current guidance says foundational SEO applies.
6. 35-45 min: select findings and draft. Internal workflows are unknown without owner input. Suggest a public-information FAQ or enquiry checklist only as an optional hypothesis, with no invented savings.
7. 45-60 min: check evidence and identity, render PDF, visual QA, human review, then deliver through the approved customer channel. Do not claim review occurred before an actual reviewer checks it.

Evidence ledger columns: finding ID; URL; source owner; checked_at_UTC; observed text; tool/method; classification; confidence reason; customer impact (inference); action; effort; priority; limitations. Keep minimum evidence excerpts, not scraped copies of entire third-party sites.

Classification required in each finding: VERIFIED FINDING (direct observation), REASONABLE INFERENCE (plausible implication), RECOMMENDATION (proposed step), UNKNOWN / UNABLE TO VERIFY. A source's claim is verified only as 'the source says X', not as proof X is true.

Priorities: Do Now = a directly verified material customer-path problem or identity conflict that the owner can address. Do Next = supported clarity/trust improvement without a demonstrated blocking issue. Later = useful but lower-confidence/lower-impact or dependency-bound improvement. Unknowns receive no severity points. Within a tier prefer higher confidence and lower effort. Do not invent financial impact or an aggregate score.

Report: 2-3 pages ordinarily; title/date/scope; concise conclusion; strengths; up to three findings with observation/evidence/implication/action/effort; Do Now/Do Next/Later (empty allowed); source links; tested and untested surfaces; limitations. State if no material issue was found. A positive result is a valid result.

## 10. Operational controls for the first ten orders

Reece remains accountable for queue checks and final approval. Check Stripe and intake/email at least at the start and end of each working period; check more frequently during an active campaign. No automatic fulfillment, alerting, or background monitoring is implied by this document. Before outreach, verify capacity to honor all orders within 24 elapsed hours, including weekends; pause the offer if capacity is exhausted.

The clock is based on max(paid_at, usable_intake_received_at), not when an operator gets around to matching them. Delayed reconciliation does not extend the customer's deadline. At 18 hours escalate unfinished work; at 24 hours offer the published remedy if late. If the form is blocked, accept business name, domain, city/state and checkout email by support email. Never request card details. Before sending a report, verify the recipient against the paid order and the customer's delivery instructions.

Honor the public refund terms: cancellation before research; duplicate charge; inability to deliver described scope; material service failure; late delivery refund on request. Correct factual errors promptly, preserve prior report versions, document reason and timestamp. Do not issue a refund or customer communication without the applicable action authorization. Never silently revise a delivered report.

Only public business material enters research prompts. Keep order emails, payment IDs and intake in private operational records. Do not commit them, put them in share links, or include them in public samples. No report publication without client consent. Review temporary research notes for deletion after support closes; keep required business/payment records under applicable obligations and provider policies. Make no unsupported retention guarantee.

## 11. Dry-run acceptance scenarios

- Paid + matching usable intake: one job, start at the later receipt timestamp.
- Open/unpaid checkout or direct visit to intake/completion: no paid status, no job.
- Paid but missing intake: queue remains awaiting intake; request only public essentials.
- $49 subtotal plus tax: valid price; tax does not cause false rejection.
- Duplicate submissions: reconcile one job, no double delivery or duplicate billing.
- Refund/dispute: hold fulfillment and escalate to Reece.
- 403, JS-only page, unavailable AI engine: report unknown/not tested; do not fabricate failure.
- Zero useful issues: honest positive report, no padded recommendations.
- Sources disagree: show dated discrepancy; ask owner to confirm before declaring truth.
- Draft says 'guaranteed rankings', 'invisible to AI', unsupported savings, or security verdict: fail QA.
- Missing source, wrong business, unverified recipient, or no visual PDF review: fail QA.


## 12. Active intake simplification (supersedes earlier Tally-first instructions)

Browser QA found unconditional payment-received text and a required personal name inside the legacy Tally form. The active canonical intake now uses email only: business name, public URL, city/state and checkout email. The Stripe redirect is unchanged. No form submission or automatic receipt is implied. Existing Tally orders still require reconciliation and must not be lost. The old external form remains outside the current website flow; no claim is made that its hosted content was edited or deactivated. Review the support inbox for subject Paid audit intake. Do not tell a buyer to use the legacy form.
