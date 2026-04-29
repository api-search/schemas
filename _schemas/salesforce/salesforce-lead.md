---
description: ''
layout: schema
name: Lead
properties_list:
- description: ''
  name: 012000000000000AAA
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-lead-schema.json
slug: salesforce-lead
source_filename: salesforce-lead-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"012000000000000AAA\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Full\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"View\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"eTag\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"id\": {\n                  \"type\": \"string\",\n                  \"example\": \"abc123\"\n                },\n                \"layoutType\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"mode\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"objectApiName\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\
  \n                },\n                \"recordTypeId\": {\n                  \"type\": \"string\",\n                  \"example\": \"500123\"\n                },\n                \"saveOptions\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                },\n                \"sections\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"collapsible\": {\n                        \"type\": \"object\"\n                      },\n                      \"columns\": {\n                        \"type\": \"object\"\n                      },\n                      \"heading\": {\n                        \"type\": \"object\"\
  \n                      },\n                      \"id\": {\n                        \"type\": \"object\"\n                      },\n                      \"layoutRows\": {\n                        \"type\": \"object\"\n                      },\n                      \"rows\": {\n                        \"type\": \"object\"\n                      },\n                      \"useHeading\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"collapsible\",\n                      \"columns\",\n                      \"heading\",\n                      \"id\",\n                      \"layoutRows\",\n                      \"rows\",\n                      \"useHeading\"\n                    ]\n                  }\n                }\n              },\n              \"required\": [\n                \"eTag\",\n                \"id\",\n                \"layoutType\",\n                \"mode\"\
  ,\n                \"objectApiName\",\n                \"recordTypeId\",\n                \"saveOptions\",\n                \"sections\"\n              ]\n            }\n          },\n          \"required\": [\n            \"View\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Full\"\n      ]\n    }\n  },\n  \"required\": [\n    \"012000000000000AAA\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Lead\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-lead-schema.json
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
title: Lead
---
