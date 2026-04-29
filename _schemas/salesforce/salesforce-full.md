---
description: ''
layout: schema
name: Full
properties_list:
- description: ''
  name: View
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-full-schema.json
slug: salesforce-full
source_filename: salesforce-full-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"View\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"eTag\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"layoutType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"mode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"objectApiName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"recordTypeId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"saveOptions\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n       \
  \ \"sections\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"collapsible\": {\n                \"type\": \"boolean\",\n                \"example\": true\n              },\n              \"columns\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"heading\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"layoutRows\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"layoutItems\": {\n\
  \                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"layoutItems\"\n                  ]\n                }\n              },\n              \"rows\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"useHeading\": {\n                \"type\": \"boolean\",\n                \"example\": true\n              }\n            },\n            \"required\": [\n              \"collapsible\",\n              \"columns\",\n              \"heading\",\n              \"id\",\n              \"layoutRows\",\n              \"rows\",\n              \"useHeading\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"eTag\",\n        \"id\",\n        \"layoutType\",\n        \"mode\",\n        \"objectApiName\",\n        \"recordTypeId\",\n        \"saveOptions\",\n        \"sections\"\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"View\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Full\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-full-schema.json
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
title: Full
---
