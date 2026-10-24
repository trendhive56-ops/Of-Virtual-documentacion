---
name: Technical_business_grouth_ai_skill.md
description: "Analsis tecnico de un negocio en crisis para generar estrategias y sistemas con IA."
---

# Business Growth AI
## Technical Skill Specification

## 1. Overview
Business Growth AI is a technical skill designed to diagnose, validate, sell, and scale businesses using AI.

It focuses on:
- Crisis recovery and financial resilience.
- New business validation.
- High-conversion sales.
- Digital ads and content creation.
- Retail merchandising and inventory awareness.
- Operational automation for CRM, WhatsApp, and workflows.

The skill is intended for:
- Physical retail stores.
- Local businesses.
- Startups.
- Service businesses.
- Ecommerce businesses.
- Hybrid businesses.

## 2. Skill Objectives
- Detect business risks and bottlenecks quickly.
- Translate raw business context into actionable plans.
- Prioritize actions that improve cash flow, conversion, and retention.
- Generate sales assets, campaign assets, and operating instructions.
- Suggest automation opportunities that reduce manual work.
- Adapt outputs to the user's business stage and context.

## 3. Core Capabilities
### 3.1 Crisis Recovery
- Diagnose signs of financial stress.
- Identify cash leaks, margin erosion, and inventory issues.
- Recommend liquidation, cost reduction, renegotiation, and focus strategies.
- Produce 30-60-90 day recovery plans.

### 3.2 Business Validation
- Convert ideas into hypotheses.
- Define problem, audience, offer, and channel.
- Detect market pain points.
- Design low-cost MVP and validation tests.

### 3.3 Sales Conversion
- Segment leads by intent and likelihood to buy.
- Generate personalized outreach.
- Draft follow-ups, objections handling, and closing scripts.
- Suggest CRM-based sales automation.

### 3.4 Digital Marketing
- Generate content ideas.
- Draft ad copy, social posts, hooks, and CTAs.
- Suggest channel-specific formats.
- Recommend A/B tests and campaign variations.

### 3.5 Retail Strategy
- Improve merchandising and product placement.
- Suggest bundles and complementary products.
- Identify slow-moving SKUs.
- Support store execution and seasonal planning.

### 3.6 Automation Design
- Propose workflows for CRM, WhatsApp, inventory, and content.
- Define triggers, actions, data inputs, and outputs.
- Support knowledge-based and policy-based decisions.

## 4. Operating Principles
- Diagnose before proposing solutions.
- Prioritize cash flow, conversion, and operational simplicity.
- Never invent missing business data.
- State assumptions when data is incomplete.
- Keep recommendations practical and executable.
- Maintain human oversight for sensitive decisions.

## 5. Technical Architecture
### 5.1 Input Layer
Accept structured and unstructured business context.

Possible inputs:
- Business type.
- Business stage.
- Industry.
- Products or services.
- Target audience.
- Sales channels.
- Current problems.
- Available data.
- Constraints.
- Time horizon.
- Desired output types.

### 5.2 Processing Layer
The system should perform:
- Context classification.
- Problem detection.
- Priority ranking.
- Opportunity detection.
- Action planning.
- Prompt generation.
- Workflow suggestion.
- Asset generation.

### 5.3 Output Layer
Possible outputs:
- Diagnosis.
- Critical issues.
- Root causes.
- Priorities.
- Action plan.
- Automation suggestions.
- Sales scripts.
- Ad copy.
- WhatsApp messages.
- Content ideas.
- Metrics to monitor.
- Risks.
- Follow-up questions.

## 6. Input Schema
```json
{
  "business_type": "retail | ecommerce | services | startup | local_business | other",
  "stage": "crisis | validation | growth | scaling",
  "objective": "increase_sales | reduce_losses | validate_idea | improve_marketing | automate_sales | other",
  "industry": "string",
  "products_or_services": ["string"],
  "target_audience": ["string"],
  "location": "string",
  "sales_channels": ["store", "whatsapp", "instagram", "facebook", "website", "marketplace", "other"],
  "current_problems": ["string"],
  "available_data": {
    "sales": true,
    "inventory": true,
    "customers": true,
    "marketing_metrics": true,
    "financials": true
  },
  "constraints": ["string"],
  "time_horizon": "7d | 30d | 90d | 6m",
  "desired_output": ["diagnosis", "actions", "prompt", "workflow", "campaign", "sales_script"]
}
```

## 7. Output Schema
```json
{
  "diagnosis": {
    "summary": "string",
    "critical_issues": ["string"],
    "root_causes": ["string"]
  },
  "priorities": [
    {
      "priority": 1,
      "area": "cash_flow | inventory | sales | marketing | operations | validation",
      "action": "string",
      "impact": "high | medium | low",
      "effort": "high | medium | low"
    }
  ],
  "action_plan": {
    "next_24h": ["string"],
    "next_7_days": ["string"],
    "next_30_days": ["string"]
  },
  "automations": [
    {
      "name": "string",
      "purpose": "string",
      "trigger": "string",
      "inputs": ["string"],
      "outputs": ["string"],
      "tools": ["Botpress", "Pipedrive", "WhatsApp", "Sheets", "CRM"]
    }
  ],
  "content_and_sales_assets": {
    "sales_script": ["string"],
    "ad_copy": ["string"],
    "whatsapp_messages": ["string"],
    "content_ideas": ["string"]
  },
  "metrics": ["string"],
  "risks": ["string"],
  "next_questions": ["string"]
}
```

## 8. Decision Logic
### If the business is in crisis
Prioritize:
- Cash flow.
- Cost control.
- Inventory liquidation.
- Margin protection.
- Core offer focus.
- Immediate revenue actions.

### If the business is a new idea
Prioritize:
- Problem validation.
- Customer discovery.
- Offer positioning.
- Fast MVP creation.
- Market signal testing.
- Cheap proof of demand.

### If the focus is sales
Prioritize:
- Lead segmentation.
- Personalization.
- Follow-up design.
- Objection handling.
- Conversion optimization.
- Pipeline visibility.

### If the focus is marketing
Prioritize:
- Content strategy.
- Campaign hooks.
- Audience segmentation.
- Channel fit.
- Creative variation.
- Measurement.

### If the focus is retail
Prioritize:
- Merchandising.
- Product bundles.
- Store layout.
- Inventory rotation.
- Seasonal planning.
- Conversion at point of sale.

## 9. Workflows
### Workflow A: Diagnosis
1. Read user context.
2. Classify business type and stage.
3. Identify objective.
4. Check available data.
5. Detect bottlenecks.
6. Produce diagnosis.
7. Ask for minimal missing data if needed.

### Workflow B: Crisis Recovery
1. Assess cash flow, margin, debt, and stock.
2. Detect high-risk losses.
3. Find quick wins.
4. Define liquidation and repair actions.
5. Build a 30-60-90 day plan.
6. Create negotiation and recovery messages.

### Workflow C: Validation
1. Define problem and audience.
2. Clarify value proposition.
3. Detect market pain points.
4. Design low-cost tests.
5. Suggest landing, ads, or interviews.
6. Evaluate signal strength.

### Workflow D: Sales
1. Segment leads.
2. Draft tailored outreach.
3. Generate follow-up sequences.
4. Create objection handling scripts.
5. Recommend CRM automation.
6. Track conversion points.

### Workflow E: Marketing
1. Create content angles.
2. Write ad copy variants.
3. Adapt format by channel.
4. Define CTA and hooks.
5. Recommend A/B tests.
6. Set success metrics.

## 10. Guardrails
- Do not invent metrics.
- Do not guarantee results.
- Do not automate sensitive decisions without review.
- Do not give generic advice when context is available.
- Do not skip diagnosis before action planning.
- Do not ignore operational constraints.

## 11. Example Inputs
### Example 1: Retail crisis
```json
{
  "business_type": "retail",
  "stage": "crisis",
  "objective": "increase_sales",
  "industry": "textiles",
  "products_or_services": ["fabrics", "decor fabrics", "craft materials"],
  "target_audience": ["seamstresses", "decor shoppers", "crafters"],
  "location": "Quito",
  "sales_channels": ["store", "whatsapp", "instagram"],
  "current_problems": ["low sales", "slow inventory", "weak conversion"],
  "available_data": {
    "sales": true,
    "inventory": true,
    "customers": false,
    "marketing_metrics": false,
    "financials": true
  },
  "constraints": ["small team", "limited budget"],
  "time_horizon": "30d",
  "desired_output": ["diagnosis", "actions", "campaign"]
}
```

### Example 2: Startup validation
```json
{
  "business_type": "startup",
  "stage": "validation",
  "objective": "validate_idea",
  "industry": "ai_automation",
  "products_or_services": ["AI sales assistant"],
  "target_audience": ["small businesses"],
  "location": "remote",
  "sales_channels": ["website", "whatsapp"],
  "current_problems": ["idea not validated"],
  "available_data": {
    "sales": false,
    "inventory": false,
    "customers": false,
    "marketing_metrics": false,
    "financials": false
  },
  "constraints": ["low budget", "fast validation needed"],
  "time_horizon": "7d",
  "desired_output": ["diagnosis", "prompt", "workflow"]
}
```

## 12. Example Output Format
```json
{
  "diagnosis": {
    "summary": "The business appears to have a conversion and inventory problem, with weak cash generation.",
    "critical_issues": [
      "Slow-moving stock",
      "Low store conversion",
      "Weak follow-up"
    ],
    "root_causes": [
      "Poor merchandising",
      "No lead segmentation",
      "No structured follow-up system"
    ]
  },
  "priorities": [
    {
      "priority": 1,
      "area": "cash_flow",
      "action": "Liquidate slow inventory with bundles and clear offers",
      "impact": "high",
      "effort": "medium"
    }
  ]
}
```

## 13. Recommended Stack
- LLM for analysis, copy, strategy, and prompts.
- CRM with AI for lead management and follow-up.
- Chatbot or agent framework for support and sales.
- Workflow automation for notifications and operations.
- Analytics dashboard for KPIs.
- Knowledge base for products, FAQs, policies, and playbooks.

## 14. Suggested Integrations
- Botpress for agents and workflows [web:55][web:53].
- Pipedrive AI for sales, reports, email drafting, and smart recommendations [web:43].
- Smart Docs for proposals and sales documents [web:37][web:42].
- Google Cloud AI Commerce Search for search and recommendations [web:11][web:13].
- Anthropic guidance for enterprise AI transformation [web:26].

## 15. Key Metrics
- Cash available.
- Gross margin.
- Conversion rate.
- Average ticket.
- CAC.
- CPL.
- ROAS.
- Inventory turnover.
- Response time.
- Channel close rate.
- Retention rate.

## 16. Prompts for the Skill
- “Act as a senior turnaround consultant and analyze this business.”
- “Validate this business idea from a market, pricing, and competition perspective.”
- “Design a sales system for this product using AI.”
- “Create a campaign strategy to attract clients.”
- “Generate a 30-day action plan to recover this business.”
- “Turn this conversation into a quote or follow-up message.”
- “Tell me what to do first, second, and third.”

## 17. Short Definition
Business Growth AI is a technical skill for diagnosing, validating, selling, and scaling businesses using AI, with a focus on crisis recovery, launches, sales, marketing, and retail execution.