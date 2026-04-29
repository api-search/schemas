---
description: Request body for batch creating calls
layout: schema
name: BatchCreateCallsRequest
properties_list:
- description: Array of calls to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-batch-create-calls-request-schema.json
slug: engagement-calls-api-batch-create-calls-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-batch-create-calls-request-schema.json\",\n  \"title\": \"BatchCreateCallsRequest\",\n  \"description\": \"Request body for batch creating calls\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of calls to create\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Request body for creating a call\",\n        \"required\": [\n          \"properties\"\n        ],\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The call properties to set\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"example\": {\n              \"hs_call_title\": \"Discovery Call\"\
  ,\n              \"hs_call_body\": \"Discussed product requirements\",\n              \"hs_call_duration\": \"1800000\",\n              \"hs_call_direction\": \"OUTBOUND\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n            }\n          },\n          \"associations\": {\n            \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationInput\"\n            },\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ]\n          }\n        }\n      },\n      \"maxItems\": 100,\n      \"example\": [\n        {\n          \"properties\": {\n            \"hs_call_title\": \"Discovery Call\",\n            \"hs_call_body\": \"Discussed product requirements\",\n            \"hs_call_duration\"\
  : \"1800000\",\n            \"hs_call_direction\": \"OUTBOUND\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-batch-create-calls-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: BatchCreateCallsRequest
---
