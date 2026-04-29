---
description: Request payload for submitting a new claim.
layout: schema
name: ClaimRequest
properties_list:
- description: Policy against which to file the claim.
  name: policy_id
  type: string
- description: Type of claim event.
  name: claim_type
  type: string
- description: Date of the qualifying event.
  name: incident_date
  type: string
- description: Description of the incident or diagnosis.
  name: description
  type: string
provider_name: aflac
provider_slug: aflac
schema_file: json-schema/enterprise-connect-claim-request-schema.json
slug: enterprise-connect-claim-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-request-schema.json\",\n  \"title\": \"ClaimRequest\",\n  \"description\": \"Request payload for submitting a new claim.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Policy against which to file the claim.\",\n      \"example\": \"POL-987654\"\n    },\n    \"claim_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of claim event.\",\n      \"enum\": [\n        \"accident\",\n        \"critical_illness\",\n        \"cancer_diagnosis\",\n        \"hospitalization\",\n        \"disability\"\n      ],\n      \"example\": \"accident\"\n    },\n    \"incident_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the qualifying event.\",\n      \"example\"\
  : \"2025-02-10\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the incident or diagnosis.\",\n      \"example\": \"Employee sustained a broken arm in a workplace accident.\"\n    }\n  },\n  \"required\": [\n    \"policy_id\",\n    \"claim_type\",\n    \"incident_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/json-schema/enterprise-connect-claim-request-schema.json
tags: []
title: ClaimRequest
---
