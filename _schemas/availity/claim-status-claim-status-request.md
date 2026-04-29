---
description: ClaimStatusRequest schema from Availity API
layout: schema
name: ClaimStatusRequest
properties_list:
- description: Availity payer ID
  name: payerId
  type: string
- description: ''
  name: provider
  type: object
- description: ''
  name: subscriber
  type: object
- description: Payer claim number
  name: claimNumber
  type: string
- description: ''
  name: fromDate
  type: string
- description: ''
  name: toDate
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-claim-status-request-schema.json
slug: claim-status-claim-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-request-schema.json\",\n  \"title\": \"ClaimStatusRequest\",\n  \"description\": \"ClaimStatusRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"provider\",\n    \"subscriber\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"description\": \"Availity payer ID\",\n      \"example\": \"BCBS001\"\n    },\n    \"provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"npi\": {\n          \"type\": \"string\",\n          \"description\": \"National Provider Identifier\",\n          \"example\": \"1234567890\"\n        },\n        \"taxId\": {\n          \"type\": \"string\",\n          \"example\": \"123456789\"\n        }\n      }\n    },\n    \"subscriber\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"memberId\": {\n          \"type\": \"string\",\n          \"example\": \"MEM123456\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"Jane\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"Smith\"\n        },\n        \"dateOfBirth\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"example\": \"1980-01-15\"\n        }\n      }\n    },\n    \"claimNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Payer claim number\",\n      \"example\": \"CLM-2025-001234\"\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-01-01\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-12-31\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-request-schema.json
tags: []
title: ClaimStatusRequest
---
