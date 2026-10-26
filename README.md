# InstaHelp: Fixing Reliability in 15-Minute Home Services
### Product Requirements Document & Case Study · by Rhea Parmar

> Independent product case study. Not affiliated with or endorsed by Urban Company. Personas and the journey map are illustrative, built from case research.

📄 **[Read the full PRD (PDF)](./PRD.pdf)**

---

## TL;DR
InstaHelp, Urban Company's 15-minute on-demand housekeeping vertical, loses **₹447 on every order** (₹9 Cr revenue against a ₹119 Cr loss in Q4 FY26), while the core scheduled-services business stays profitable. The cause is not demand but **reliability**. I proposed a recovery-first solution: when a professional cancels, the system automatically rematches the booking or hands the customer to a human, so no customer is left in a dead end.

---

## 1. Problem
- Partners cancel bookings at the last minute.
- Customers get stuck in an unresolvable chatbot loop when that happens.
- Some bookings are marked "complete" even though no professional arrived.
- InstaHelp charges a **30–40% premium** over competitors like Snabbit and Pronto. That premium is only justified if the service is more dependable, and today it is not.

## 2. Goals and non-goals
**Goals**
1. Eliminate the unresolvable chatbot loop: every cancellation resolves to an automated rematch or a human handoff.
2. Stop bookings from being marked "complete" without verified service delivery.

**Non-goals**
1. Not a supply-acquisition effort: no need to hire more partners.
2. Not touching Core Services: the scheduled-booking business is already profitable.

## 3. Success metrics
| Type | Metric | Target |
|---|---|---|
| **North Star** | Contribution Margin per Order | –₹447 (Q4 FY26) → toward ₹0, phased |
| L1 | Partner Cancellation Rate | Baseline TBD; target set once instrumented |
| L1 | Post-Cancellation Resolution Rate | Baseline TBD; target set once instrumented |
| L1 | Verified Completion Rate | Baseline TBD; target set once instrumented |
| L1 | CSAT after Cancellation Recovery | Baseline TBD; target set once instrumented |
| Retention | D30 (Day-30) Retention | Baseline TBD; the real test of whether recovery rebuilds trust |
| Counter-metrics | Partner Acceptance Rate, Support Cost per Order | Must not decline or spike as fixes roll out |

## 4. User personas
**Meera, the Emergency User (primary).** A dual-income household professional in a metro city who needs a backup when her regular helper is unavailable. She wants a backup that shows up, instant and honest status updates, and zero extra coordination on an already hard morning.

**Rohan, the Reliability Shopper (secondary).** A price-aware, early-career professional who compares apps before booking and has no proof of reliability. He wants a visible reliability score, transparent pricing tied to service quality, and a reason to stop comparing apps every time.

![User personas](./images/personas.png)

## 5. User journey
Mapped across Awareness → Consideration → Onboarding → Retention → Loyalty. The biggest pain points sit at **Retention** ("They cancelled again") and **Consideration** ("Can't find ratings").

| # | Stage | Opportunity | Impact |
|---|---|---|---|
| 1 | Retention | Auto-rematch on cancellation | Time-to-rematch (Effort: S) |
| 2 | Onboarding | Predictive partner pre-positioning | Cancellation rate (Effort: M) |
| 3 | Consideration | Live reliability score | Conversion rate (Effort: S) |
| 4 | Loyalty | Loyalty rewards for rebooking | D30 retention (Effort: M) |

![Customer journey map](./images/journey-map.png)

## 6. Solution options and prioritisation
| Opportunity | Reach | Impact | Confidence | Effort | Priority |
|---|---|---|---|---|---|
| **AI Real-Time Recovery** | High | High | High | Medium | **P0** |
| Reliability-Tiered Subscription | High | High | Medium | High | P1 |
| Partner Incentive & Reliability Model | Medium | Medium | Medium | Medium | P2 |

- **AI Real-Time Recovery (P0):** automatically recover a booking by finding an alternative professional, without the customer rebooking.
- **Reliability-Tiered Subscription (P1):** plans with benefits tied to consistent fulfilment and recovery.
- **Partner Incentive & Reliability Model (P2):** align partner incentives with acceptance, fulfilment and reliability.

**Why recovery first?** It has the highest reach, impact and confidence, and it directly closes the "dead-end chatbot" failure that damages trust most.

## 7. Requirements

### Functional
1. **Cancellation detection:** detect when an assigned professional cancels an active booking before service starts.
2. **Automatic booking recovery:** identify and assign an eligible alternative professional without the customer rebooking.
3. **Failure recovery and customer resolution:** if no replacement is available, notify the customer clearly and give an immediate resolution, such as cancellation and refund.

### Non-functional
| Category | Requirement |
|---|---|
| Performance | 95% of eligible cancellations trigger a recovery attempt within 30 seconds |
| Quality | Recover ≥80% of eligible cancelled bookings, subject to professional availability |
| Reliability | Recovery works without the customer restarting or recreating the booking |
| Security | Data protected by the existing authentication, authorisation and data-security controls |
| Transparency | Every cancellation, attempt, reassignment, failure and final outcome is recorded in an auditable event log |
| Usability | Customer needs no more than 2 interactions to accept or decline a recovery option |

## 8. Mock-ups and prototype
*Coming soon:* [add screenshots here, or link your Figma file]

---

## Skills demonstrated
Problem framing · Metrics definition (North Star, L1, counter-metrics) · Persona and journey mapping · RICE prioritisation · Requirements writing (functional and non-functional) · Competitive thinking

📧 rheaparmar19dec@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/rhea-parmar-837a6a16a/)
