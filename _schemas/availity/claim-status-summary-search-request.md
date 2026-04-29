---
description: SummarySearchRequest schema from Availity API
layout: schema
name: SummarySearchRequest
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: requestType
  type: string
- description: ''
  name: memberId
  type: string
- description: ''
  name: fromDate
  type: string
- description: ''
  name: toDate
  type: string
- description: ''
  name: providerNpi
  type: string
- description: ''
  name: checkNumber
  type: string
- description: ''
  name: requestedStatus
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-summary-search-request-schema.json
slug: claim-status-summary-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-summary-search-request-schema.json\",\n  \"title\": \"SummarySearchRequest\",\n  \"description\": \"SummarySearchRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"requestType\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"requestType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVICE_DATE\",\n        \"MEMBER_ID\"\n      ],\n      \"example\": \"SERVICE_DATE\"\n    },\n    \"memberId\": {\n      \"type\": \"string\",\n      \"example\": \"MEM123456\"\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-01-01\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date\",\n      \"example\": \"2025-12-31\"\n    },\n    \"providerNpi\": {\n      \"type\": \"string\",\n      \"example\": \"1234567890\"\n    },\n    \"checkNumber\": {\n      \"type\": \"string\",\n      \"example\": \"CHK-001234\"\n    },\n    \"requestedStatus\": {\n      \"type\": \"string\",\n      \"example\": \"PAID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-summary-search-request-schema.json
tags: []
title: SummarySearchRequest
---
