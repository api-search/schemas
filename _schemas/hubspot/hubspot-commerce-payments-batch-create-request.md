---
description: Request body for batch creating commerce payments
layout: schema
name: BatchCreateRequest
properties_list:
- description: List of payments to create
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-batch-create-request-schema.json
slug: hubspot-commerce-payments-batch-create-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for batch creating commerce payments\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"List of payments to create\",\n      \"example\": [\n        {\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"associations\": [\n            {\n              \"to\": {\n                \"id\": {}\n              },\n              \"types\": [\n                {}\n              ]\n            }\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for creating a new commerce payment\",\n        \"properties\": {\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The properties to set on the commerce payment\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"associations\": {\n   \
  \         \"type\": \"array\",\n            \"description\": \"Associations to create with other objects\",\n            \"example\": [\n              {\n                \"to\": {\n                  \"id\": {}\n                },\n                \"types\": [\n                  {}\n                ]\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"Input for creating an association\",\n              \"properties\": {\n                \"to\": {\n                  \"type\": \"object\",\n                  \"example\": {\n                    \"id\": \"500123\"\n                  },\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\"\n                  ]\n                },\n                \"types\": {\n                  \"type\": \"array\",\n  \
  \                \"description\": \"The association types\",\n                  \"example\": [\n                    {\n                      \"associationCategory\": \"HUBSPOT_DEFINED\",\n                      \"associationTypeId\": 500123\n                    }\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"to\",\n                \"types\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"properties\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-batch-create-request-schema.json
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
title: BatchCreateRequest
---
