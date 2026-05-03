---
description: Schema for a SaaS application subscription managed within the Sastrify platform
layout: schema
name: SaaSSubscription
properties_list:
- description: Unique identifier for the subscription record in Sastrify
  name: id
  type: string
- description: Name of the SaaS application
  name: applicationName
  type: string
- description: Name of the SaaS vendor or publisher
  name: vendorName
  type: string
- description: Functional category of the SaaS tool
  name: category
  type: string
- description: Annual cost of the subscription in the contract currency
  name: annualCost
  type: number
- description: ISO 4217 currency code for the annual cost
  name: currency
  type: string
- description: Total number of licenses or seats in the current contract
  name: licenseCount
  type: integer
- description: Number of users active in the past 30 days
  name: activeUsers
  type: integer
- description: Percentage of provisioned licenses actively used (activeUsers / licenseCount)
  name: utilizationRate
  type: number
- description: Contract renewal date
  name: renewalDate
  type: string
- description: Start date of the current contract term
  name: contractStartDate
  type: string
- description: Payment schedule for the subscription
  name: paymentTerms
  type: string
- description: Whether the contract auto-renews at expiration
  name: autoRenew
  type: boolean
- description: Name or email of the internal owner responsible for this subscription
  name: contractOwner
  type: string
- description: Primary business department using this tool
  name: department
  type: string
- description: Market pricing benchmark for this tool category
  name: benchmarkData
  type: object
- description: How the subscription was discovered by Sastrify
  name: discoverySource
  type: string
- description: Current status of the subscription in Sastrify
  name: status
  type: string
provider_name: Sastrify
provider_slug: sastrify
schema_file: json-schema/sastrify-saas-subscription-schema.json
slug: sastrify-saas-subscription
source_filename: sastrify-saas-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sastrify/main/json-schema/sastrify-saas-subscription-schema.json\",\n  \"title\": \"SaaSSubscription\",\n  \"description\": \"Schema for a SaaS application subscription managed within the Sastrify platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the subscription record in Sastrify\",\n      \"example\": \"sub_01HXYZ1234567890\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SaaS application\",\n      \"example\": \"Salesforce\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SaaS vendor or publisher\",\n      \"example\": \"Salesforce, Inc.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Functional category\
  \ of the SaaS tool\",\n      \"example\": \"CRM\",\n      \"enum\": [\n        \"CRM\",\n        \"Communication\",\n        \"Project Management\",\n        \"HR\",\n        \"Finance\",\n        \"Security\",\n        \"Analytics\",\n        \"Design\",\n        \"Development\",\n        \"Marketing\",\n        \"Legal\",\n        \"IT Operations\",\n        \"Document Management\",\n        \"Collaboration\",\n        \"Other\"\n      ]\n    },\n    \"annualCost\": {\n      \"type\": \"number\",\n      \"description\": \"Annual cost of the subscription in the contract currency\",\n      \"minimum\": 0,\n      \"example\": 120000\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the annual cost\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"example\": \"USD\"\n    },\n    \"licenseCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of licenses or seats in the current contract\",\n      \"minimum\"\
  : 1,\n      \"example\": 200\n    },\n    \"activeUsers\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users active in the past 30 days\",\n      \"minimum\": 0,\n      \"example\": 145\n    },\n    \"utilizationRate\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of provisioned licenses actively used (activeUsers / licenseCount)\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 72.5\n    },\n    \"renewalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Contract renewal date\",\n      \"example\": \"2026-12-31\"\n    },\n    \"contractStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the current contract term\",\n      \"example\": \"2025-01-01\"\n    },\n    \"paymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment schedule for the subscription\",\n      \"example\": \"Annual Prepaid\",\n\
  \      \"enum\": [\"Annual Prepaid\", \"Monthly\", \"Quarterly\", \"Multi-Year\"]\n    },\n    \"autoRenew\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contract auto-renews at expiration\",\n      \"example\": true\n    },\n    \"contractOwner\": {\n      \"type\": \"string\",\n      \"description\": \"Name or email of the internal owner responsible for this subscription\",\n      \"example\": \"jane.smith@example.com\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Primary business department using this tool\",\n      \"example\": \"Sales\"\n    },\n    \"benchmarkData\": {\n      \"type\": \"object\",\n      \"description\": \"Market pricing benchmark for this tool category\",\n      \"properties\": {\n        \"medianPricePerSeat\": {\n          \"type\": \"number\",\n          \"description\": \"Median market price per seat per year for this tool category\",\n          \"example\": 560\n        },\n        \"organizationPricePerSeat\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"Current price per seat per year paid by the organization\",\n          \"example\": 600\n        },\n        \"savingsOpportunity\": {\n          \"type\": \"number\",\n          \"description\": \"Estimated annual savings if price is brought to benchmark\",\n          \"example\": 8000\n        },\n        \"percentile\": {\n          \"type\": \"integer\",\n          \"description\": \"Price percentile (e.g., 75 means paying more than 75% of similar companies)\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"example\": 72\n        }\n      }\n    },\n    \"discoverySource\": {\n      \"type\": \"string\",\n      \"description\": \"How the subscription was discovered by Sastrify\",\n      \"example\": \"SSO Integration\",\n      \"enum\": [\n        \"SSO Integration\",\n        \"Accounting Integration\",\n        \"Browser Extension\",\n        \"Manual Entry\",\n        \"Email Integration\"\n\
  \      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the subscription in Sastrify\",\n      \"example\": \"Active\",\n      \"enum\": [\"Active\", \"Pending Renewal\", \"Cancelled\", \"Under Review\", \"In Negotiation\"]\n    }\n  },\n  \"required\": [\"applicationName\", \"vendorName\", \"annualCost\", \"currency\", \"licenseCount\", \"renewalDate\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sastrify/refs/heads/main/json-schema/sastrify-saas-subscription-schema.json
tags:
- Cost Optimization
- License Management
- Procurement
- SaaS Management
- Software Spend
- Vendor Management
title: SaaSSubscription
---
