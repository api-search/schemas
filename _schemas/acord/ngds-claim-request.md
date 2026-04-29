---
description: ClaimRequest schema from ACORD NGDS API
layout: schema
name: ClaimRequest
properties_list:
- description: ''
  name: policyId
  type: string
- description: ''
  name: lossDate
  type: string
- description: ''
  name: lossDescription
  type: string
- description: ''
  name: lossLocation
  type: object
- description: ''
  name: claimant
  type: object
- description: ''
  name: estimatedLossAmount
  type: number
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-claim-request-schema.json
slug: ngds-claim-request
source_filename: ngds-claim-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-claim-request-schema.json\",\n  \"title\": \"ClaimRequest\",\n  \"description\": \"ClaimRequest schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\"\n    },\n    \"lossDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"lossDescription\": {\n      \"type\": \"string\"\n    },\n    \"lossLocation\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"claimant\": {\n      \"$ref\": \"#/components/schemas/PartyRequest\"\n    },\n    \"estimatedLossAmount\": {\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"policyId\",\n    \"lossDate\",\n    \"lossDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-claim-request-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: ClaimRequest
---
