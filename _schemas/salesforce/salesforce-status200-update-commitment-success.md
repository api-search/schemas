---
description: ''
layout: schema
name: Status200-UpdateCommitmentSuccess
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: links
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status200-update-commitment-success-schema.json
slug: salesforce-status200-update-commitment-success
source_filename: salesforce-status200-update-commitment-success-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"giftcommitment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        },\n        \"giftcommitmentschedule\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n    \
  \      },\n          \"required\": [\n            \"href\",\n            \"id\"\n          ]\n        }\n      },\n      \"required\": [\n        \"giftcommitment\",\n        \"giftcommitmentschedule\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"links\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status200-UpdateCommitmentSuccess\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status200-update-commitment-success-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Status200-UpdateCommitmentSuccess
---
