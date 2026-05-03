---
description: Schema for a regulatory compliance check result, as returned by RegTech APIs for ongoing compliance monitoring and reporting.
layout: schema
name: Regulatory Compliance Check
properties_list:
- description: Unique identifier for this compliance check.
  name: checkId
  type: string
- description: Identifier of the entity being checked for compliance.
  name: entityId
  type: string
- description: Name of the entity being checked.
  name: entityName
  type: string
- description: Regulatory framework being checked against (e.g., 'GDPR', 'HIPAA', 'MiFID II', 'SOC2').
  name: framework
  type: string
- description: Regulatory jurisdiction (e.g., 'US', 'EU', 'UK').
  name: jurisdiction
  type: string
- description: Date and time the compliance check was performed.
  name: checkDate
  type: string
- description: Overall compliance status.
  name: status
  type: string
- description: Individual compliance findings.
  name: findings
  type: array
- description: Overall compliance score as a percentage.
  name: score
  type: number
- description: URL to the full compliance report.
  name: reportUrl
  type: string
provider_name: Regulatory
provider_slug: regulatory
schema_file: json-schema/regulatory-compliance-check-schema.json
slug: regulatory-compliance-check
source_filename: regulatory-compliance-check-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regulatory/json-schema/regulatory-compliance-check-schema.json\",\n  \"title\": \"Regulatory Compliance Check\",\n  \"description\": \"Schema for a regulatory compliance check result, as returned by RegTech APIs for ongoing compliance monitoring and reporting.\",\n  \"type\": \"object\",\n  \"required\": [\"checkId\", \"entityId\", \"framework\", \"checkDate\", \"status\"],\n  \"properties\": {\n    \"checkId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this compliance check.\"\n    },\n    \"entityId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the entity being checked for compliance.\"\n    },\n    \"entityName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the entity being checked.\"\n    },\n    \"framework\": {\n      \"type\": \"string\",\n      \"description\": \"Regulatory\
  \ framework being checked against (e.g., 'GDPR', 'HIPAA', 'MiFID II', 'SOC2').\"\n    },\n    \"jurisdiction\": {\n      \"type\": \"string\",\n      \"description\": \"Regulatory jurisdiction (e.g., 'US', 'EU', 'UK').\"\n    },\n    \"checkDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the compliance check was performed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall compliance status.\",\n      \"enum\": [\"Compliant\", \"Non-Compliant\", \"Partial\", \"Under Review\", \"Unknown\"]\n    },\n    \"findings\": {\n      \"type\": \"array\",\n      \"description\": \"Individual compliance findings.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"findingId\", \"controlId\", \"status\"],\n        \"properties\": {\n          \"findingId\": {\n            \"type\": \"string\"\n          },\n          \"controlId\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"Reference to the specific compliance control checked.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\"Pass\", \"Fail\", \"Warning\", \"Not Applicable\"]\n          },\n          \"evidence\": {\n            \"type\": \"string\",\n            \"description\": \"Evidence supporting this finding.\"\n          },\n          \"remediationRequired\": {\n            \"type\": \"boolean\"\n          },\n          \"remediationDeadline\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          }\n        }\n      }\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall compliance score as a percentage.\"\n    },\n    \"reportUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full compliance report.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regulatory/refs/heads/main/json-schema/regulatory-compliance-check-schema.json
tags:
- Compliance
- Financial Services
- Governance
- Healthcare Regulation
- Regulatory Reporting
- Risk Management
- RegTech
title: Regulatory Compliance Check
---
