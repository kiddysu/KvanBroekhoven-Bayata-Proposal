# Risk Analysis

## Critical Risks (Kill Project if Not Mitigated)

### 1. Agent Architecture Fails at Scale
**Risk:** Claude agent doesn't work in production (rate limiting, API issues, webhook delays).
**Probability:** 30-40%
**Kill Signal:** Week 2 discovery endpoint broken OR Week 5 load test crashes
**Mitigation:** Build incrementally (Week 1: discovery only, 50 prospects). Week 5: stress test with 5,000 prospects before Month 1.
**Fallback:** Manual CSV + Zapier (slower, but functional).

---

### 2. The company Bayata Deprioritizes API Development
**Risk:** Bayata says yes but doesn't deliver APIs (engineering busy with paying customers).
**Probability:** 40-50%
**Kill Signal:** No API spec by end of Week 1 OR API delivery slips >1 week. Move forward with other API's as there are other options, but inform the company Bayata
**Mitigation:** Demand written API spec + dedicated owner + weekly updates + €500/week delay penalty in contract or move on with API's i can use for the agents.
**Fallback:** CSV export from the company Bayata (not ideal, keeps project moving).

---

### 3. Prospect Data Quality Is Bad
**Risk:** 40% invalid emails, wrong contacts, outdated info = email open rate 8% (not 24%).
**Probability:** 25-35%
**Kill Signal:** Email delivery rate <80% after 200 test sends OR 30% bounces
**Mitigation:** Validate 200 prospects in Week 1. If delivery <85%: request data refresh before pilot.And search for another option besides Lusha
**Fallback:** Manually source 50-100 high-quality prospects from LinkedIn.

---

## High Risks (Manageable But Serious)

### 4. Close Rate Is 50% Below Forecast
**Risk:** Actual 0.6% close rate (not 1.25%) = 11 closes (not 60).
**Probability:** 25-30%
**Kill Signal:** <0.5% close rate after 1,000 prospects OR <0.3% after 500
**Mitigation:** Month 1 hypothesis testing (send 100 test emails, measure actual close rate). Kill bad segments immediately. Weekly performance audits.
**Fallback:** Pivot to different product (PlateOptimizer instead of Mestloket).

---

### 6. The company Bayata Doesn't Support You
**Risk:** Slow responses (3-5 days), vague answers, no dedicated person = blocked waiting.
**Probability:** 25-30%
**Kill Signal:** No response to critical issue >4 hours OR the company Bayata misses 2 weekly meetings
**Mitigation:** Demand dedicated point person (Week 1). Escalation to VP if missed.
**Fallback:** Work around them (manual workarounds, don't wait).

---

## Medium Risks (Possible But Manageable)

### 7. Payment Disputes (The company Bayata Won't Pay Commission)
**Risk:** Bayata disputes closes: "These customers are low quality" or "Let's pay after 90 days instead of Month 1."
**Probability:** 10-20%
**Kill Signal:** First payment delayed >1 week OR Bayata demands "quality audit" before paying
**Mitigation:** Define "close" objectively in contract (contract signed + payment received). Churn clawback max 30 days only. Monthly invoicing + 15-day payment SLA.
**Fallback:** Legal escalation (arbitration clause in contract).

---

### 8. Agent Costs More Than Expected
**Risk:** Real costs €2,000/month: Claude API (€1.5K),, enrichment (€500), infrastructure (€500).
**Probability:** 15-25%
**Kill Signal:** Monthly costs >€1,000 by Month 2 OR cost per close >€150 by Month 3
**Mitigation:** Track spend weekly from Week 1. Optimize API usage (batch calls, cache data). Cap tooling spend. Build cost model by Month 2.
**Fallback:** Renegotiate commission rate with the company Bayata if CAC too high and during and after the pilot phase.

---

## Monthly Checkpoint Checklist

**Weeks 1-4 (Technical):** Can you build agent? APIs ready?
**Weeks 5-8 (Market):** Data quality good? Close rate on track?
**Weeks 9-12 (Operational):** Burnout signs? The company Bayata responsive? Payments on time?

If ANY kill signal appears: Stop, escalate, renegotiate or kill.

---

*File 10: Risk Analysis · KvanBroekhoven · April 2026*