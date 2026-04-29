---
description: Request body for creating a call
layout: schema
name: CallCreateRequest
properties_list:
- description: The call properties to set
  name: properties
  type: object
- description: Associations to create with other objects
  name: associations
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-call-create-request-schema.json
slug: engagement-calls-api-call-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-create-request-schema.json\",\n  \"title\": \"CallCreateRequest\",\n  \"description\": \"Request body for creating a call\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The call properties to set\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"hs_call_title\": \"Discovery Call\",\n        \"hs_call_body\": \"Discussed product requirements\",\n        \"hs_call_duration\": \"1800000\",\n        \"hs_call_direction\": \"OUTBOUND\",\n        \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"Associations to create with other objects\",\n      \"items\": {\n\
  \        \"type\": \"object\",\n        \"description\": \"Association to create with another object\",\n        \"required\": [\n          \"to\",\n          \"types\"\n        ],\n        \"properties\": {\n          \"to\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"id\"\n            ],\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the object to associate with\",\n                \"example\": \"101\"\n              }\n            },\n            \"example\": {\n              \"id\": \"101\"\n            }\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"description\": \"The association types\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationType\"\n            },\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n    \
  \            \"associationTypeId\": 194\n              }\n            ]\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"to\": {\n            \"id\": {}\n          },\n          \"types\": [\n            {}\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-create-request-schema.json
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
title: CallCreateRequest
---
