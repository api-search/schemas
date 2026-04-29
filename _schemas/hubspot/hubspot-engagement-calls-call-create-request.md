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
schema_file: json-schema/hubspot-engagement-calls-call-create-request-schema.json
slug: hubspot-engagement-calls-call-create-request
source_filename: hubspot-engagement-calls-call-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a call\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The call properties to set\",\n      \"example\": {\n        \"hs_call_title\": \"Discovery Call\",\n        \"hs_call_body\": \"Discussed product requirements\",\n        \"hs_call_duration\": \"1800000\",\n        \"hs_call_direction\": \"OUTBOUND\",\n        \"hs_timestamp\": \"2024-01-15T10:30:00.000Z\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"Associations to create with other objects\",\n      \"example\": [\n        {\n          \"to\": {\n            \"id\": {}\n          },\n          \"types\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Association to create with another object\",\n        \"properties\": {\n          \"to\": {\n            \"\
  type\": \"object\",\n            \"example\": {\n              \"id\": \"101\"\n            },\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the object to associate with\",\n                \"example\": \"101\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"description\": \"The association types\",\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 194\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Type of association\",\n              \"properties\": {\n                \"associationCategory\": {\n                  \"type\": \"string\",\n                  \"description\": \"The category\
  \ of association\",\n                  \"example\": \"HUBSPOT_DEFINED\",\n                  \"enum\": [\n                    \"HUBSPOT_DEFINED\",\n                    \"USER_DEFINED\",\n                    \"INTEGRATOR_DEFINED\"\n                  ]\n                },\n                \"associationTypeId\": {\n                  \"type\": \"integer\",\n                  \"description\": \"The association type ID\",\n                  \"example\": 194\n                }\n              },\n              \"required\": [\n                \"associationCategory\",\n                \"associationTypeId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"to\",\n          \"types\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-call-create-request-schema.json
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
