# Sales Funnel AI
## Technical Skill Specification

## 1. Overview
Sales Funnel AI is a technical skill designed to build, optimize, and automate sales funnels that consistently acquire, qualify, nurture, and convert clients.

It works across:
- Physical retail.
- Local businesses.
- Ecommerce.
- Services.
- Startups.
- B2B and B2C operations.

The skill is meant to connect:
- Traffic acquisition.
- Lead capture.
- Qualification.
- Nurture.
- Sales conversion.
- Retention.
- Re-engagement.

## 2. Main Purpose
- Structure the client acquisition process.
- Turn business context into a working funnel.
- Reduce manual follow-up.
- Improve lead quality and conversion.
- Align marketing, sales, and automation.
- Create repeatable systems that work for different business models.

## 3. Core Funnel Logic
A funnel should move a prospect through these stages:
1. Awareness.
2. Interest.
3. Qualification.
4. Consideration.
5. Conversion.
6. Retention.
7. Re-engagement.

The skill must identify:
- Where the funnel starts.
- What channel attracts the lead.
- What data is captured.
- How the lead is scored.
- What action moves the lead forward.
- What triggers follow-up.
- What closes the sale.
- What brings the client back.

## 4. Funnel Types
### 4.1 Retail Funnel
For physical stores and product-based businesses.
- Traffic to store or WhatsApp.
- Product discovery.
- Offer or bundle.
- Purchase.
- Repeat purchase.

### 4.2 Lead Generation Funnel
For services, agencies, B2B, and consulting.
- Ad or content click.
- Form submission or chat start.
- Qualification.
- Meeting or demo.
- Proposal.
- Close.

### 4.3 Ecommerce Funnel
- Ad or organic entry.
- Product view.
- Add to cart.
- Abandoned cart recovery.
- Checkout.
- Post-purchase.

### 4.4 Startup Validation Funnel
- Problem awareness.
- Landing page.
- Waitlist or form.
- Discovery call.
- Pilot.
- Early adopters.

### 4.5 WhatsApp Funnel
- Entry from social, store, ad, or referral.
- Conversation start.
- Need identification.
- Product or service matching.
- Quote or offer.
- Close.
- Follow-up.

## 5. Technical Capabilities
### 5.1 Lead Capture
- Create entry points from website, WhatsApp, social media, store, forms, ads, or QR codes.
- Capture contact data and context.
- Route leads into the correct funnel branch.

### 5.2 Lead Qualification
- Score leads by intent, urgency, budget, fit, and engagement.
- Filter out low-quality leads early.
- Prioritize leads most likely to buy.
- Ask adaptive qualifying questions.

### 5.3 Nurture Automation
- Send personalized messages based on stage and behavior.
- Trigger reminders, educational content, and offers.
- Re-engage silent leads.
- Move leads automatically when criteria are met.

### 5.4 Sales Conversion
- Generate offers, quotes, bundles, proposals, and closing scripts.
- Support negotiation and objection handling.
- Track deal movement.
- Detect stalled opportunities.

### 5.5 Retention and Re-Engagement
- Send post-sale follow-ups.
- Promote cross-sell and upsell.
- Recover inactive clients.
- Trigger loyalty and repeat purchase campaigns.

## 6. Funnel Architecture
### Input Layer
The skill should accept:
- Business type.
- Industry.
- Product or service.
- Target audience.
- Sales channels.
- Traffic sources.
- Current funnel stage.
- Offer structure.
- Lead capture method.
- CRM or automation stack.
- Constraints.
- Goal.

### Processing Layer
The system should:
- Classify the funnel type.
- Map the customer journey.
- Detect leaks.
- Score leads.
- Recommend actions.
- Generate sequences.
- Suggest automation.
- Define KPIs.

### Output Layer
The system should produce:
- Funnel map.
- Lead scoring logic.
- Stage-by-stage actions.
- Messages and scripts.
- Automated workflows.
- Campaign structure.
- KPI dashboard.
- Optimization plan.

## 7. Input Schema
```json
{
  "business_type": "retail | ecommerce | services | startup | local_business | other",
  "funnel_type": "retail | lead_generation | ecommerce | validation | whatsapp",
  "industry": "string",
  "products_or_services": ["string"],
  "target_audience": ["string"],
  "sales_channels": ["store", "whatsapp", "instagram", "facebook", "website", "email", "ads", "marketplace"],
  "traffic_sources": ["organic", "paid", "referral", "in_store", "social", "search"],
  "current_funnel_stage": "awareness | interest | qualification | consideration | conversion | retention | reengagement",
  "lead_capture_methods": ["form", "chat", "whatsapp", "call", "store_visit", "dm"],
  "offer_structure": ["string"],
  "current_problems": ["string"],
  "available_data": {
    "traffic": true,
    "leads": true,
    "crm": true,
    "sales": true,
    "inventory": true,
    "marketing_metrics": true
  },
  "constraints": ["string"],
  "time_horizon": "7d | 30d | 90d | 6m",
  "desired_output": ["funnel_map", "lead_scoring", "messages", "workflow", "campaign", "kpis"]
}
```

## 8. Output Schema
```json
{
  "funnel_summary": {
    "type": "string",
    "goal": "string",
    "main_leak": "string"
  },
  "funnel_map": [
    {
      "stage": "string",
      "objective": "string",
      "entry_actions": ["string"],
      "exit_criteria": ["string"]
    }
  ],
  "lead_scoring": {
    "criteria": ["string"],
    "high_score_threshold": 0,
    "qualified_lead_definition": "string"
  },
  "automation_plan": [
    {
      "name": "string",
      "trigger": "string",
      "action": "string",
      "tools": ["Botpress", "Pipedrive", "WhatsApp", "CRM", "Email"]
    }
  ],
  "sales_assets": {
    "messages": ["string"],
    "follow_up_sequences": ["string"],
    "sales_script": ["string"],
    "objection_handling": ["string"],
    "offer_variants": ["string"]
  },
  "optimization": {
    "kpis": ["string"],
    "bottlenecks": ["string"],
    "tests": ["string"]
  },
  "next_questions": ["string"]
}
```

## 9. Funnel Building Rules
- Every funnel must have a clear entry point.
- Every stage must have an exit criterion.
- Every lead must have a scoring mechanism.
- Every channel must map to a stage.
- Every nurture step must have a purpose.
- Every conversion step must be measurable.
- Every dropped lead must have a re-engagement path.
- Every funnel must include review and optimization.

## 10. Funnel Design by Business Stage
### If the business is in crisis
Prioritize:
- Fast cash generation.
- Offers with immediate conversion.
- WhatsApp and direct response.
- Inventory liquidation.
- Retention of existing clients.

### If the business is launching
Prioritize:
- Awareness and validation.
- Waitlist or interest capture.
- Small paid tests.
- Clear proposition.
- Early adopter follow-up.

### If the business is growing
Prioritize:
- Lead scoring.
- Nurture sequences.
- Pipeline visibility.
- Conversion optimization.
- Retention automation.

### If the business is scaling
Prioritize:
- Segmented funnels.
- CRM automation.
- Multi-channel orchestration.
- Predictive lead prioritization.
- Dashboards and revenue ops.

## 11. Workflow Design
### Workflow A: Funnel Diagnosis
1. Identify business type.
2. Identify funnel type.
3. Map current acquisition path.
4. Detect where leads stop.
5. Find weakest stage.
6. Propose fixes.

### Workflow B: Funnel Creation
1. Define ICP.
2. Define offer.
3. Define traffic source.
4. Define capture mechanism.
5. Define qualification steps.
6. Define nurture sequence.
7. Define conversion action.
8. Define retention flow.

### Workflow C: Funnel Optimization
1. Review conversion at each stage.
2. Detect drop-off points.
3. Adjust copy and offers.
4. Test variations.
5. Improve scoring.
6. Refine automation.

### Workflow D: Funnel Automation
1. Trigger lead capture.
2. Apply scoring.
3. Route lead.
4. Send sequences.
5. Notify sales.
6. Track conversion.
7. Re-engage inactive leads.

## 12. Automation Examples
### Example 1: WhatsApp lead funnel
- Trigger: user writes to WhatsApp.
- Action: bot asks qualifying questions.
- Next step: assign score.
- If qualified: send offer and book meeting.
- If not qualified: send educational sequence.

### Example 2: Retail funnel
- Trigger: visitor scans QR or messages store.
- Action: identify product interest.
- Next step: recommend bundles.
- If interested: send price and close.
- If no response: follow-up reminder.

### Example 3: Startup funnel
- Trigger: visit landing page.
- Action: capture email or WhatsApp.
- Next step: send validation message.
- If positive: schedule call.
- If not ready: add to nurture.

## 13. KPI Framework
- Traffic by channel.
- Lead capture rate.
- Qualification rate.
- Response time.
- Meeting booked rate.
- Proposal sent rate.
- Conversion rate.
- Average order value.
- Repeat purchase rate.
- Win rate by stage.
- Funnel drop-off rate.
- Re-engagement rate.

## 14. Guardrails
- Do not use funnel automation without clear exit criteria.
- Do not send generic nurture to high-value leads.
- Do not score leads only by demographics.
- Do not ignore the role of human follow-up in high-ticket sales.
- Do not optimize only for lead volume if lead quality is poor.
- Do not leave retention out of the funnel.

## 15. Tooling Recommendations
- Pipedrive AI for CRM, scoring, follow-up, and sales productivity [web:58][web:43].
- Botpress for lead generation, qualification, and automated interaction [web:63][web:47][web:53].
- Smart Docs for proposals and contracts [web:37][web:42].
- Email automation and scheduling tools for nurture and meetings.
- Analytics tools for funnel visibility and optimization.

## 16. Prompt Templates
- “Design a sales funnel for this business.”
- “Map the client journey from awareness to conversion.”
- “Create lead scoring rules for this funnel.”
- “Build WhatsApp follow-up messages for each funnel stage.”
- “Identify where leads are dropping out of the funnel.”
- “Design a retention and reactivation sequence.”
- “Create a 30-day funnel optimization plan.”

## 17. Short Definition
Sales Funnel AI is a technical skill for building structured client acquisition systems that capture, qualify, nurture, convert, retain, and re-engage leads using AI, CRM, and automation.