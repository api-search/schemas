---
description: PartyRequest schema from ACORD NGDS API
layout: schema
name: PartyRequest
properties_list:
- description: ''
  name: partyType
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: organizationName
  type: string
- description: ''
  name: taxId
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: contacts
  type: array
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/ngds-party-request-schema.json
slug: ngds-party-request
source_filename: ngds-party-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-party-request-schema.json\",\n  \"title\": \"PartyRequest\",\n  \"description\": \"PartyRequest schema from ACORD NGDS API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Insured\",\n        \"Claimant\",\n        \"Agent\",\n        \"Broker\",\n        \"Carrier\"\n      ]\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Contact\"\n      }\n    }\n \
  \ },\n  \"required\": [\n    \"partyType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/ngds-party-request-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: PartyRequest
---
