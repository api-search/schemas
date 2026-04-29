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
schema_file: json-schema/hubspot-engagement-calls-batch-create-calls-request-schema.json
slug: hubspot-engagement-calls-batch-create-calls-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch creating calls\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of calls to create\",\n      \"example\": [\n        {\n          \"properties\": {\n            \"hs_call_title\": \"Discovery Call\",\n            \"hs_call_body\": \"Discussed product requirements\",\n            \"hs_call_duration\": \"1800000\",\n            \"hs_call_direction\": \"OUTBOUND\",\n            \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Request body for creating a call\",\n        \"properties\": {\n          \"properties\": {\n            \"type\"\
  : \"object\",\n            \"description\": \"The call properties to set\",\n            \"example\": {\n              \"hs_call_title\": \"Discovery Call\",\n              \"hs_call_body\": \"Discussed product requirements\",\n              \"hs_call_duration\": \"1800000\",\n              \"hs_call_direction\": \"OUTBOUND\",\n              \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n            }\n          },\n          \"associations\": {\n            \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Association to create with another object\",\n              \"properties\": {\n                \"to\": {\n        \
  \          \"type\": \"object\",\n                  \"example\": {\n                    \"id\": \"101\"\n                  },\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\"\n                  ]\n                },\n                \"types\": {\n                  \"type\": \"array\",\n                  \"description\": \"The association types\",\n                  \"example\": [\n                    {\n                      \"associationCategory\": \"HUBSPOT_DEFINED\",\n                      \"associationTypeId\": 194\n                    }\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"to\",\n                \"types\"\n              ]\n            }\n          }\n\
  \        },\n        \"required\": [\n          \"properties\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCreateCallsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-batch-create-calls-request-schema.json
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
