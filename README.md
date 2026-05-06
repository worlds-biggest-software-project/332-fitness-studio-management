# Fitness Studio Management

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An open, AI-native platform for class booking, membership billing, instructor scheduling, and retail — built for boutique studios that are tired of opaque pricing, multi-week onboarding, and vendor lock-in.

Fitness Studio Management is a candidate open-source platform for independent gyms, boutique studios, and multi-location operators. It unifies group class scheduling, recurring membership billing, member self-service, and in-studio retail in a single system, and applies AI to the operational decisions — capacity, retention, scheduling — that today require either expensive enterprise tiers or guesswork.

---

## Why Fitness Studio Management?

- **Incumbents are expensive and opaque.** Mindbody runs $139–$699+/month with a ~2.75% transaction fee on top; Glofox, Zingfit, Pike13, Wodify, TeamUp and Hapana all use undisclosed custom pricing, and Zen Planner's advertised $99/month routinely exceeds $447/month once add-ons are layered in.
- **Onboarding takes weeks.** Setup complexity is a documented top reason studios abandon software, with Mindbody in particular drawing complaints about multi-week onboarding and a steep learning curve.
- **AI is gated to premium tiers — or absent.** Only Hapana offers meaningful AI-driven churn scoring and engagement analytics; most platforms have no native capability at all, leaving smaller studios without access to retention intelligence.
- **Data is locked in.** Studio owners cannot easily export or analyse their own data across the major platforms, and the only existing open-source entry — GYM One (MIT) — is rudimentary, with no mobile app, no analytics, and no marketing automation.
- **Mixed-model studios are underserved.** Studios running both group classes and personal training routinely operate two systems because no incumbent handles both well in one unified scheduler.

---

## Key Features

### Scheduling & Booking

- Group class scheduling with recurring templates, capacity limits, and exception handling
- Waitlist management with automatic member promotion and notifications
- Online booking via embeddable widget and mobile-friendly web app
- Unified scheduler covering both group classes and personal training appointments
- Seat/equipment-position selection booking for cycling, rowing, and similar formats (using non-trademarked terminology)

### Membership, Billing & Retail

- Recurring membership billing with automated failed-payment retry (dunning)
- Customisable membership plan builder covering plans, pricing, and access rules
- Member self-service portal for booking, cancellation, payment, and history
- POS and basic retail inventory for in-studio sales and merchandise
- PCI DSS compliant payment processing

### Member Experience & Engagement

- Attendance tracking with front desk, kiosk, and app-based check-in
- Email and SMS notification automation for reminders, failed payments, and re-engagement
- White-label or branded mobile app for iOS and Android
- Hybrid digital/on-demand class delivery and virtual content library
- Wearable and fitness device data ingestion

### Operations & Analytics

- Reporting dashboards covering revenue, attendance trends, and membership health
- Staff scheduling, payroll reporting, and permission roles
- Multi-location and franchise management with centralised reporting
- Performance and workout tracking module with personal record boards

---

## AI-Native Advantage

AI is applied to the operational decisions that drive studio economics: a churn-prediction model trained on attendance patterns surfaces at-risk members weeks before they cancel; a dynamic capacity engine adjusts class caps and waitlist promotions based on historical no-show rates and predicted demand; instructor assignments are correlated with fill rates, member ratings, and revenue to surface optimal scheduling and flag burnout risk. LLM-assisted programme design generates class templates adapted to studio niche, member progression data, and ACSM safety guidelines, while retail demand forecasting predicts merchandise and supplement stock from attendance trends.

---

## Tech Stack & Deployment

The platform is designed to be self-hostable (mirroring the open-source posture of GYM One but with a modern feature set) as well as deployable as a managed cloud service. Integrations follow the open-API pattern adopted by Glofox, Hapana, Pike13, and TeamUp, with REST endpoints and webhooks for booking, payment, and membership events, plus connectors for Stripe, Zapier, QuickBooks, Mailchimp, and wearable/fitness data sources. Architecture targets ACSM Health/Fitness Facility Standards, IHRSA operational benchmarks, ADA accessibility requirements, and PCI DSS for payment handling.

---

## Market Context

The fitness studio management software market was valued at approximately USD 1.5 billion in 2024 and is forecast to reach USD 3.5 billion by 2033 at a ~9.7% CAGR (Verified Market Reports); the broader gym management software segment is on track from USD 2.03 billion in 2025 to USD 4.02 billion by 2032 at 10.24% CAGR (Business Research Insights). Cloud-based platforms now account for roughly 57% of usage, North America holds over 40% market share, and the buyer base spans solo trainers and boutique operators (Vagaro, Pike13, TeamUp price points) through to franchise chains and enterprise multi-location brands (ClubReady, Mindbody, ABC Fitness/Glofox).

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

Note: "Spot Scheduling®" is a registered trademark of Zingfit/Mariana Tek. Use neutral terminology such as "seat selection booking" or "equipment reservation" in any contributed code, UI copy, or documentation.

---

## Licence

Licence to be determined. See [discussion](#) for context.
