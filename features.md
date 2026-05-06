# Fitness Studio Management — Feature & Functionality Survey

> Candidate #332 · Researched: 2026-05-03

## Solutions Analysed

| Tool | Type | Licence / Model | URL |
|------|------|-----------------|-----|
| Mindbody | All-in-one SaaS | Commercial — subscription ($139–$699+/mo) | https://www.mindbodyonline.com |
| Vagaro | All-in-one SaaS | Commercial — per-staff pricing ($30+/mo) | https://www.vagaro.com |
| Glofox (ABC Fitness) | Boutique SaaS | Commercial — subscription (custom pricing) | https://abcfitness.com/glofox/ |
| Zen Planner | Niche SaaS | Commercial — subscription ($99+/mo) | https://zenplanner.com |
| Zingfit / Mariana Tek | Boutique SaaS | Commercial — subscription (custom pricing) | https://zingfit.com |
| Pike13 | SMB SaaS | Commercial — subscription (custom pricing) | https://www.pike13.com |
| Wodify | CrossFit/Functional SaaS | Commercial — subscription (custom pricing) | https://www.wodify.com |
| TeamUp | Independent studio SaaS | Commercial — subscription (custom pricing) | https://goteamup.com |
| Hapana | AI-native SaaS | Commercial — subscription (custom pricing) | https://www.hapana.com |
| GYM One | Open source | Open source (MIT) | https://github.com/mayerbalintdev/GYM-One |

---

## Feature Analysis by Solution

### Mindbody

**Core features**
- Multi-resource class scheduling (rooms, equipment, instructors) with recurring and one-off templates
- Waitlist management with automatic promotion and member notifications
- Series and workshops with separate multi-session registration
- Recurring membership billing with automatic failed-payment retry (dunning)
- Branded mobile app for member booking, payments, and communications
- Marketing tools including automated campaigns and email sequences
- Reporting dashboard covering attendance, revenue, and retention metrics
- POS and retail inventory management
- Staff scheduling and payroll reporting
- ClassPass and third-party marketplace integrations

**Differentiating features**
- Largest consumer marketplace network (Mindbody app) driving new member discovery
- AI-powered scheduling recommendations and demand forecasting
- Multi-location and franchise architecture

**UX patterns**
- Tiered onboarding with a dedicated setup wizard; complexity managed via plan gating
- Member-facing booking via Mindbody consumer app, website widget, or direct link
- Staff dashboard with drag-and-drop schedule builder

**Integration points**
- Public REST API via developer portal (developers.mindbodyonline.com)
- ClassPass, Zapier, Mailchimp, QuickBooks, Perkville loyalty programme
- Webhooks for booking, payment, and membership events

**Known gaps**
- High base cost; key features (branded app, advanced marketing) locked to expensive tiers
- Steep learning curve; onboarding can take weeks
- Transaction fee (~2.75%) on top of subscription adds up for high-volume studios
- Support quality complaints at lower tiers

**Licence / IP notes**
- Proprietary SaaS; no open-source components. Spot Booking® terminology trademarked by Zingfit/Mariana Tek.

---

### Vagaro

**Core features**
- Group class scheduling with capacity limits, waitlists, and series
- 24/7 online booking via Vagaro marketplace, website widget, or embeddable calendar
- Integrated POS with multi-payment support (cash, card, mobile payments)
- Built-in payroll module tied to time tracking and appointment data
- Inventory management with real-time tracking
- Client profiles with history, photos, notes, and payment records
- Automated invoicing and recurring billing
- Two-way calendar sync (Google, Outlook, iCal)

**Differentiating features**
- Native payroll processing within the same platform — unique among mid-market tools
- Consumer-facing Vagaro marketplace for member acquisition
- Low per-staff pricing model accessible to solo trainers and small studios

**UX patterns**
- Simple admin dashboard with drag-and-drop scheduling
- Progressive add-ons model — start simple, layer in features as needed
- Self-service client portal and mobile app

**Integration points**
- Google Calendar, Outlook, iCal sync
- Zapier automation
- Power BI, Salesforce, Tableau, NetSuite for business intelligence export
- QuickBooks for accounting

**Known gaps**
- Less suitable for high-end boutique brands requiring deep white-label customisation
- Analytics less sophisticated than Glofox or Hapana
- Limited franchise/multi-location architecture compared to enterprise tools

**Licence / IP notes**
- Proprietary SaaS; no open-source components.

---

### Glofox (ABC Fitness)

**Core features**
- Member management with full lifecycle view from sign-up to renewal
- Class scheduling with automated billing and recurring payment management
- Branded white-label member app with class booking, payment management, and community features
- Attendance and engagement analytics with churn risk surfacing
- Reporting on membership sales, attendance rates, and failed payments
- Multi-location support across 100+ countries and 17 languages
- Push notification and in-app messaging for member communications
- Staff management and access control

**Differentiating features**
- Deep retention analytics surfacing members at drop-off risk early
- White-label branded app as a standard offering (not an expensive add-on)
- Integration with ABC Fitness enterprise ecosystem post-acquisition

**UX patterns**
- Clean mobile-first design with a strong emphasis on member self-service
- Dashboard designed around retention metrics rather than operational tasks
- Onboarding flow guided by a dedicated success manager

**Integration points**
- Open API with 40+ partner integrations
- ClassPass, Zapier, Mailchimp, and payment gateways (Stripe-based)
- Wearable device data ingestion for attendance and workout tracking

**Known gaps**
- Pricing is not published; custom quotes can be expensive for small studios
- Limited depth in payroll, accounting, and retail POS compared to Vagaro
- Some users report sluggish performance on the admin dashboard

**Licence / IP notes**
- Proprietary SaaS; acquired by ABC Fitness, so roadmap governed by larger corporate entity.

---

### Zen Planner

**Core features**
- Recurring membership billing with auto-renewals and flexible plan structures (monthly, annual, custom)
- Belt and skill progression tracking for martial arts schools
- Testing event management and rank advancement workflows
- Member self-service portal with online bill payment
- Online class scheduling with embeddable calendar widget
- Automated check-in via member app
- Online retail store module
- Staff management and payroll reporting
- PCI-DSS compliant payment processing

**Differentiating features**
- Belt tracking and rank progression purpose-built for martial arts — unmatched depth in this niche
- Functional fitness and CrossFit programming support alongside martial arts
- Average transaction fees 15% below competitors per their own claims

**UX patterns**
- Workflow-driven interface optimised for front desk staff
- Member portal for self-service payment, scheduling, and progress review
- Marketing module (Engage) as a separate add-on

**Integration points**
- QuickBooks integration for accounting
- Engage marketing module (add-on)
- Website and branded app as paid add-ons

**Known gaps**
- Base price appears low ($99/mo) but real cost with add-ons often exceeds $447/mo
- Consumer-facing design is less polished than Mindbody or Glofox
- Limited appeal outside of martial arts, CrossFit, and functional fitness niches
- Less sophisticated analytics compared to Hapana or Glofox

**Licence / IP notes**
- Proprietary SaaS; no open-source components.

---

### Zingfit / Mariana Tek

**Core features**
- Spot Scheduling® — proprietary system for booking a specific piece of equipment (bike, mat position)
- Online scheduling with auto-enrolling waitlists
- Studio management with payroll, reporting, and staff tools
- POS and e-commerce functionality
- Client management with booking history
- Marketing tools integrated into the scheduling flow

**Differentiating features**
- Spot Scheduling® is genuinely unique — members pick a specific bike or mat position during booking
- Built exclusively for boutique group fitness (cycling, yoga, HIIT) — not a generalised tool
- Strong brand customisation for studios where experience design is the product

**UX patterns**
- Highly branded member-facing experience that reflects studio identity
- Lightweight admin interface optimised for class-centric operations
- Spot selection UI designed to feel like choosing a cinema seat

**Integration points**
- Integration with Mariana Tek (parent platform post-rebranding)
- Payment gateway and POS integrations

**Known gaps**
- Narrowly focused — unsuitable for studios running mixed class/PT/retail operations
- Limited analytical depth compared to Hapana or Glofox
- Unclear roadmap post-integration into Mariana Tek

**Licence / IP notes**
- Proprietary SaaS. "Spot Scheduling®" is a registered trademark — avoid replicating the name in any competing product.

---

### Pike13

**Core features**
- Schedule and enrolment management for group classes and private sessions
- Attendance tracking, roster management, and no-show reduction tools
- Automated invoicing, recurring billing, and integrated payment processing
- Client profiles with history, photos, notes, schedules, and payment records
- Staff payroll with variable rates, tips, bonuses, and commissions
- Text and email notifications for account issues and class reminders
- Reporting dashboards for attendance trends, membership revenue, and staff performance

**Differentiating features**
- Dedicated onboarding specialist for every new customer — high white-glove setup support
- Robust API with good developer documentation — easier to build custom integrations
- Equally suited to fitness, dance, and multi-discipline activity businesses

**UX patterns**
- Clean, minimal interface that reduces cognitive load for front desk staff
- Self-service client payment update flow reduces admin overhead
- Default dashboards surface critical metrics without configuration

**Integration points**
- REST API with documented endpoints
- Zapier for workflow automation
- Payment gateways (card processing integrated)

**Known gaps**
- Less brand visibility compared to Mindbody or Vagaro — harder to attract walk-in or marketplace members
- No built-in consumer marketplace; studios must drive their own member acquisition
- Marketing automation less mature than Mindbody or Glofox

**Licence / IP notes**
- Proprietary SaaS; no open-source components. API is documented but proprietary.

---

### Wodify

**Core features**
- Class scheduling and automated billing for CrossFit, functional fitness, jiu-jitsu, and boutique studios
- Digital Whiteboard — members log workout scores, view class leaderboards, and track personal records
- PERFORM module for workout performance tracking, PR tracking, and belt/rank progression
- CRM with member communication and retention tools
- Mobile app for members with booking, score logging, and community features
- Mobile retail with in-app purchasing
- Reporting dashboard: 16% average income increase cited by customers using analytics
- Staff management and payroll

**Differentiating features**
- Digital Whiteboard replacing gym dry-erase boards is central to CrossFit culture and community
- Performance tracking depth (PRs, progressions, ranking) is unmatched in the CrossFit niche
- Built natively for CrossFit affiliate requirements — not a general tool retrofitted

**UX patterns**
- Community-centric UX with social elements (leaderboards, shared PRs) driving daily engagement
- Workout-first member experience rather than scheduling-first
- Score logging interface optimised for fast mobile entry post-WOD

**Integration points**
- Integration with Stripe for payments
- Zapier for workflow automation
- Open API for custom integrations

**Known gaps**
- Limited appeal outside CrossFit and functional fitness; less competitive for yoga, cycling, or dance
- UI design can feel dated in the admin console
- Less sophisticated marketing automation compared to Mindbody or Glofox

**Licence / IP notes**
- Proprietary SaaS; no open-source components.

---

### TeamUp

**Core features**
- Customisable membership plan builder (plans, pricing, access rules)
- Group class, appointment, and course scheduling
- Recurring payment processing with automated renewals
- Multi-location support with centralised dashboard
- Attendance tracking and waitlist management
- Financial reporting and attendance trend analysis
- Zapier integrations for workflow automation
- Free data import service for new customers
- POS functionality

**Differentiating features**
- Transparent, usage-based pricing published openly — no surprise fees
- Courses and multi-session workshops as a first-class booking type
- Free import service reduces switching friction significantly

**UX patterns**
- Straightforward admin dashboard with minimal learning curve
- Embeddable booking widget for studio websites
- Member self-service portal for schedule management and payments

**Integration points**
- Zapier (broad automation ecosystem)
- GoCardless and Stripe for payments
- Mailchimp for email marketing
- Open API

**Known gaps**
- Branded member app available but less polished than Glofox or Hapana
- Analytics and retention intelligence less sophisticated than AI-native platforms
- Less marketing automation depth than Mindbody

**Licence / IP notes**
- Proprietary SaaS; no open-source components.

---

### Hapana

**Core features**
- White-label branded member app with class booking, payment management, and self check-in
- AI-powered member engagement analytics: behaviour, preferences, and engagement scoring
- Fitness challenges and milestone reward system to drive retention
- On-demand virtual content and at-home workout delivery
- Real-time reporting on member engagement, revenue, and growth areas
- Automated membership billing and renewal management
- Digital kiosk check-in support
- Push notifications and in-app messaging
- Feedback collection tools within the member app

**Differentiating features**
- AI/ML-driven attendance prediction and churn risk scoring — most advanced of all surveyed tools
- Challenges and rewards gamification built natively into the member app
- 40+ integrations via open API as a stated platform commitment
- White-label app is a standard feature, not a premium add-on

**UX patterns**
- Member experience designed around habit formation and community, not just transactions
- Gamification elements (challenges, milestones, rewards) embedded throughout the member journey
- Admin dashboard oriented around engagement health scores rather than operational lists

**Integration points**
- 40+ integrations via open API
- Payment gateways, CRM tools, marketing platforms
- Wearable and third-party fitness data ingestion

**Known gaps**
- Custom pricing (not published) — likely expensive for small independent studios
- Operations-heavy features (payroll, POS, inventory) less developed than Vagaro
- Relatively new entrant; long-term platform stability less proven than Mindbody or Vagaro

**Licence / IP notes**
- Proprietary SaaS; no open-source components.

---

### GYM One

**Core features**
- Member management and registration
- Basic class scheduling
- Attendance tracking
- Payment recording

**Differentiating features**
- Freely available open-source codebase — operators can self-host and customise
- No per-seat or transaction fees

**UX patterns**
- Minimal UI; primarily functional rather than polished

**Integration points**
- Open codebase — integrations must be self-built
- No pre-built third-party connectors

**Known gaps**
- Feature set is rudimentary compared to commercial alternatives
- No mobile app, marketing automation, AI features, or analytics
- Requires technical expertise to deploy, host, and maintain
- No community support at scale

**Licence / IP notes**
- MIT licence. Freely usable, modifiable, and redistributable. No patent concerns identified.

---

## Cross-Cutting Feature Themes

### Table-Stakes Features
- Group class scheduling with recurring templates and exception handling
- Online booking via website widget, mobile app, and/or consumer marketplace
- Waitlist management with automatic member promotion and notification
- Recurring membership billing with automated failed-payment retry
- Member self-service portal (view schedule, make payments, update profile)
- Attendance tracking and check-in (front desk, kiosk, or app-based)
- Reporting dashboards covering revenue, attendance, and membership health
- Staff management and basic payroll reporting
- POS for in-studio retail and service add-ons
- Email and SMS notifications for bookings, reminders, and account alerts

### Differentiating Features
- White-label branded member app (Glofox, Hapana — standard; Mindbody — premium add-on)
- Spot/seat selection booking (Zingfit — unique, trademarked)
- Digital workout whiteboard and performance tracking (Wodify — CrossFit niche)
- Belt/rank progression tracking for martial arts (Zen Planner)
- Native payroll processing (Vagaro — unique among SaaS tools)
- AI-driven churn prediction and engagement scoring (Hapana — most advanced)
- Consumer marketplace for organic member discovery (Mindbody, Vagaro)
- Course and multi-session workshop booking as first-class type (TeamUp)

### Underserved Areas / Opportunities
- **Class + PT in one platform**: Most tools serve group classes or personal training well, but rarely both without friction — studios running mixed models often use two systems
- **Transparent, predictable pricing**: Many platforms advertise low entry prices but real costs (add-ons, transaction fees, branded app) are significantly higher; studios distrust pricing
- **Fast onboarding**: Complexity and multi-week setup remain the top reason studios abandon software — simpler configuration flows are needed
- **Open, composable data access**: Studio owners cannot easily export or analyse their own data; vendor lock-in is a common complaint
- **Wearable and biometric integration**: Demand exists but only Hapana and a few others offer meaningful device data ingestion
- **Hybrid digital/physical class management**: 85% of members expect some digital access; most tools treat this as an afterthought
- **AI-assisted programming**: LLM-generated workout templates and adaptive programming based on member progress data is nascent but in demand
- **Cross-studio membership portability**: Members attending multiple studio brands under one account/pass is poorly served

### AI-Augmentation Candidates
- **Churn prediction**: Attendance pattern analysis to surface at-risk members before they cancel (Hapana leads; most platforms have no native capability)
- **Dynamic class capacity optimisation**: Adjusting caps and waitlist promotions based on predicted demand and historical no-show rates
- **Smart scheduling recommendations**: Matching instructor assignments to demand, fill rates, and member preferences automatically
- **Personalised re-engagement messaging**: Generating and timing outreach messages based on individual member behaviour rather than bulk campaigns
- **AI-assisted workout programme design**: LLM-generated class programming templates adapted to niche, member progression, and safety guidelines (ACSM)
- **Retail and inventory demand forecasting**: Predicting merchandise and supplement stock requirements from attendance trends
- **Automated onboarding guidance**: Conversational AI to walk new studio owners through configuration rather than requiring multi-week support engagements

---

## Legal & IP Summary

All major commercial platforms (Mindbody, Vagaro, Glofox, Zen Planner, Zingfit, Pike13, Wodify, TeamUp, Hapana) are proprietary SaaS products. No GPL or copyleft licences are in play for any of the leading commercial tools. The only meaningful open-source entry — GYM One — is MIT-licensed and poses no IP risk. One trademark concern is relevant: "Spot Scheduling®" is a registered trademark of Zingfit/Mariana Tek and refers specifically to their seat/equipment selection booking feature — a competing product should use different terminology (e.g., "seat selection booking" or "equipment reservation"). No software patents were identified in the research. Standard data portability and privacy obligations (GDPR, CCPA, PCI DSS) apply to any platform handling member payment and personal data.

---

## Recommended Feature Scope

**Must-have (MVP)**
- Group class scheduling with recurring templates, capacity limits, and waitlist management
- Online booking via embeddable widget and mobile-friendly web app
- Recurring membership billing with automated failed-payment retry
- Member self-service portal (book, cancel, pay, view history)
- Attendance tracking and front desk check-in
- Basic reporting: revenue, attendance trends, membership health dashboard

**Should-have (v1.1)**
- Native white-label or branded mobile app for iOS and Android
- Appointment booking for personal training alongside group classes (unified scheduler)
- AI-driven churn risk scoring surfacing at-risk members automatically
- Staff scheduling, payroll reporting, and permission roles
- POS and basic retail inventory for in-studio sales
- Email and SMS notification automation (reminders, failed payments, re-engagement)

**Nice-to-have (backlog)**
- Spot/seat selection booking for equipment-based classes (cycling, rowing)
- Performance and workout tracking module with personal record boards
- Hybrid digital/on-demand class delivery and virtual content library
- Wearable and fitness device data ingestion
- AI-assisted workout programme template generation
- Multi-location and franchise management with centralised reporting
