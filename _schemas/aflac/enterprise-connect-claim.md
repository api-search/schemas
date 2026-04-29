---
description: A supplemental insurance claim record.
layout: schema
name: Claim
properties_list:
- description: Unique claim identifier.
  name: claim_id
  type: string
- description: Policy associated with the claim.
  name: policy_id
  type: string
- description: Claimant employee identifier.
  name: employee_id
  type: string
- description: Type of claim event.
  name: claim_type
  type: string
- description: Current claim processing status.
  name: status
  type: string
- description: Date of the qualifying event.
  name: incident_date
  type: string
- description: Timestamp when the claim was submitted.
  name: submission_date
  type: string
- description: Approved benefit payment amount in USD.
  name: benefit_amount
  type: number
- description: Reason for denial if the claim was denied.
  name: denial_reason
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-claim-schema.json
slug: enterprise-connect-claim
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-schema.json\",\n  \"title\": \"Claim\",\n  \"description\": \"A supplemental insurance claim record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"claim_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique claim identifier.\",\n      \"example\": \"CLM-112233\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Policy associated with the claim.\",\n      \"example\": \"POL-987654\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Claimant employee identifier.\",\n      \"example\": \"EMP-789012\"\n    },\n    \"claim_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of claim event.\",\n      \"enum\": [\n        \"accident\",\n        \"critical_illness\",\n        \"cancer_diagnosis\"\
  ,\n        \"hospitalization\",\n        \"disability\"\n      ],\n      \"example\": \"accident\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current claim processing status.\",\n      \"enum\": [\n        \"submitted\",\n        \"in_review\",\n        \"approved\",\n        \"denied\",\n        \"paid\"\n      ],\n      \"example\": \"approved\"\n    },\n    \"incident_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the qualifying event.\",\n      \"example\": \"2025-02-10\"\n    },\n    \"submission_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the claim was submitted.\",\n      \"example\": \"2025-02-15T09:30:00Z\"\n    },\n    \"benefit_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Approved benefit payment amount in USD.\",\n      \"example\": 1500.0\n    },\n    \"denial_reason\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Reason for denial if the claim was denied.\",\n      \"example\": \"Condition not covered under policy terms.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-schema.json
tags: []
title: Claim
---
