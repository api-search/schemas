---
description: An affiliate referral event tracking a publisher's referral of a customer to acehardware.com via the Impact affiliate network.
layout: schema
name: AceHardwareAffiliateReferral
properties_list:
- description: Unique identifier for this referral event
  name: referralId
  type: string
- description: Impact affiliate account identifier
  name: affiliateId
  type: string
- description: Name of the affiliate publisher
  name: affiliateName
  type: string
- description: URL of the affiliate's referring page
  name: referralUrl
  type: string
- description: Ace Hardware product page the customer was referred to
  name: destinationUrl
  type: string
- description: Date and time the affiliate link was clicked
  name: clickDate
  type: string
- description: Date and time the purchase was completed
  name: conversionDate
  type: string
- description: Ace Hardware order identifier from the converted sale
  name: orderId
  type: string
- description: Total order value in USD
  name: orderValue
  type: number
- description: Commission percentage earned by the affiliate
  name: commissionRate
  type: number
- description: Commission amount earned in USD
  name: commissionAmount
  type: number
- description: Status of the commission
  name: status
  type: string
provider_name: Ace Hardware
provider_slug: ace-hardware
schema_file: json-schema/ace-hardware-affiliate-referral-schema.json
slug: ace-hardware-affiliate-referral
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/json-schema/ace-hardware-affiliate-referral-schema.json\",\n  \"title\": \"AceHardwareAffiliateReferral\",\n  \"description\": \"An affiliate referral event tracking a publisher's referral of a customer to acehardware.com via the Impact affiliate network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"referralId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this referral event\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"affiliateId\": {\n      \"type\": \"string\",\n      \"description\": \"Impact affiliate account identifier\",\n      \"example\": \"AFF-500123\"\n    },\n    \"affiliateName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the affiliate publisher\",\n      \"example\": \"Home\
  \ Improvement Blog\"\n    },\n    \"referralUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the affiliate's referring page\",\n      \"example\": \"https://www.homeimprovementblog.com/best-hammers\"\n    },\n    \"destinationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Ace Hardware product page the customer was referred to\",\n      \"example\": \"https://www.acehardware.com/departments/tools/hand-tools/hammers\"\n    },\n    \"clickDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the affiliate link was clicked\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    },\n    \"conversionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the purchase was completed\",\n      \"example\": \"2026-04-19T11:15:00Z\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Ace Hardware order identifier from the converted sale\",\n      \"example\": \"ORD-2026-789012\"\n    },\n    \"orderValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total order value in USD\",\n      \"example\": 89.97\n    },\n    \"commissionRate\": {\n      \"type\": \"number\",\n      \"description\": \"Commission percentage earned by the affiliate\",\n      \"example\": 4.5\n    },\n    \"commissionAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Commission amount earned in USD\",\n      \"example\": 4.05\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the commission\",\n      \"enum\": [\"Pending\", \"Approved\", \"Rejected\", \"Paid\"],\n      \"example\": \"Approved\"\n    }\n  },\n  \"required\": [\"referralId\", \"affiliateId\", \"clickDate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ace-hardware/refs/heads/main/json-schema/ace-hardware-affiliate-referral-schema.json
tags:
- Retail
- Hardware
- Home Improvement
- Tools
- Paint
- Cooperative
- EDI
- Affiliate
title: AceHardwareAffiliateReferral
---
