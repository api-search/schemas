---
description: ''
layout: schema
name: IntentEnrich
properties_list:
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: totalResults
  type: integer
- description: ''
  name: currentPage
  type: integer
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-intent-enrich-schema.json
slug: zoominfo-intent-enrich
source_filename: zoominfo-intent-enrich-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"topic\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"signalScore\": {\n            \"type\": \"integer\",\n            \"example\": 85\n          },\n          \"audienceStrength\": {\n            \"type\"\
  : \"string\",\n            \"example\": \"example_value\"\n          },\n          \"newSignal\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"signalDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"trend\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"recommendedContacts\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"firstName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"lastName\": {\n                  \"type\": \"string\",\n\
  \                  \"example\": \"Acme Corporation\"\n                },\n                \"jobTitle\": {\n                  \"type\": \"string\",\n                  \"example\": \"Vice President of Sales\"\n                },\n                \"jobFunction\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"id\",\n                \"firstName\",\n                \"lastName\",\n                \"jobTitle\",\n                \"jobFunction\"\n              ]\n            }\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"name\": {\n                \"\
  type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"website\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"hasOtherTopicConsumption\": {\n                \"type\": \"boolean\",\n                \"example\": true\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\",\n              \"website\",\n              \"hasOtherTopicConsumption\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"category\",\n          \"topic\",\n          \"signalScore\",\n          \"audienceStrength\",\n          \"newSignal\",\n          \"signalDate\",\n          \"trend\",\n          \"recommendedContacts\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\",\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntentEnrich\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-intent-enrich-schema.json
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
title: IntentEnrich
---
