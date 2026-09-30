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
Stripe paid order + Tally intake submission.

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

### Different Stripe and Tally emails
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
