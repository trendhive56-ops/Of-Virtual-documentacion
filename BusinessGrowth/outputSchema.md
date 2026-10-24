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