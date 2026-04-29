---
description: ClaimStatusResponse schema from Availity API
layout: schema
name: ClaimStatusResponse
properties_list:
- description: Availity transaction ID
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: traceIds
  type: object
- description: ''
  name: amounts
  type: object
- description: ''
  name: completeCode
  type: string
- description: ''
  name: errors
  type: array
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-claim-status-response-schema.json
slug: claim-status-claim-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-response-schema.json\",\n  \"title\": \"ClaimStatusResponse\",\n  \"description\": \"ClaimStatusResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Availity transaction ID\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACKNOWLEDGED\",\n        \"ACTION_REQUIRED\",\n        \"ADJUSTED\",\n        \"CAPITATED\",\n        \"DENIED\",\n        \"ERROR\",\n        \"FINALIZED\",\n        \"PAID\",\n        \"PENDING\",\n        \"REJECTED\",\n        \"RETURNED_TO_PROVIDER\"\n      ],\n      \"example\": \"PAID\"\n    },\n    \"traceIds\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AVAILITY_TRACE_ID\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4\"\n        },\n        \"PAYER_TRACE_ID\": {\n          \"type\": \"string\",\n          \"example\": \"277-trace-001\"\n        }\n      }\n    },\n    \"amounts\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"billed\": {\n          \"type\": \"number\",\n          \"example\": 250.0\n        },\n        \"allowed\": {\n          \"type\": \"number\",\n          \"example\": 200.0\n        },\n        \"paid\": {\n          \"type\": \"number\",\n          \"example\": 160.0\n        },\n        \"patientResponsibility\": {\n          \"type\": \"number\",\n          \"example\": 40.0\n        }\n      }\n    },\n    \"completeCode\": {\n      \"type\": \"string\",\n      \"example\": \"COMPLETE\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": {\n            \"type\"\
  : \"string\"\n          },\n          \"message\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-claim-status-response-schema.json
tags: []
title: ClaimStatusResponse
---
