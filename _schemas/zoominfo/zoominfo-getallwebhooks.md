---
description: ''
layout: schema
name: Getallwebhooks
properties_list:
- description: ''
  name: webhooks
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-getallwebhooks-schema.json
slug: zoominfo-getallwebhooks
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhooks\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"targetUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          },\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"subscriptions\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"\
  items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"createdDate\": {\n                  \"type\": \"string\",\n                  \"example\": \"2025-03-15T14:30:00Z\"\n                },\n                \"modifiedDate\": {\n                  \"type\": \"string\",\n                  \"example\": \"2025-03-15T14:30:00Z\"\n                },\n                \"eventType\": {\n                  \"type\": \"string\",\n                  \"example\": \"standard\"\n                },\n                \"objectType\": {\n                  \"type\": \"string\",\n                  \"example\": \"standard\"\n                },\n                \"fullPayload\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"subscriptionId\": {\n                  \"type\": \"string\",\n                  \"example\": \"500123\"\n                }\n              },\n              \"required\": [\n \
  \               \"createdDate\",\n                \"modifiedDate\",\n                \"eventType\",\n                \"objectType\",\n                \"subscriptionId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"enabled\",\n          \"targetUrl\",\n          \"createdDate\",\n          \"subscriptions\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"webhooks\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Getallwebhooks\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-getallwebhooks-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Getallwebhooks
---
