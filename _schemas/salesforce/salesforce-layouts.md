---
description: ''
layout: schema
name: Layouts
properties_list:
- description: ''
  name: Lead
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-layouts-schema.json
slug: salesforce-layouts
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lead\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"012000000000000AAA\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Full\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"View\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"eTag\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    },\n                    \"id\": {\n                      \"type\": \"string\",\n                      \"example\": \"abc123\"\n                    },\n                    \"layoutType\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    },\n                    \"mode\": {\n                      \"type\": \"string\",\n                      \"example\"\
  : \"example_value\"\n                    },\n                    \"objectApiName\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    },\n                    \"recordTypeId\": {\n                      \"type\": \"string\",\n                      \"example\": \"500123\"\n                    },\n                    \"saveOptions\": {\n                      \"type\": \"array\",\n                      \"description\": \"\",\n                      \"example\": [],\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"sections\": {\n                      \"type\": \"array\",\n                      \"description\": \"\",\n                      \"example\": [],\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    }\n                  },\n            \
  \      \"required\": [\n                    \"eTag\",\n                    \"id\",\n                    \"layoutType\",\n                    \"mode\",\n                    \"objectApiName\",\n                    \"recordTypeId\",\n                    \"saveOptions\",\n                    \"sections\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"View\"\n              ]\n            }\n          },\n          \"required\": [\n            \"Full\"\n          ]\n        }\n      },\n      \"required\": [\n        \"012000000000000AAA\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Lead\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Layouts\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-layouts-schema.json
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
title: Layouts
---
