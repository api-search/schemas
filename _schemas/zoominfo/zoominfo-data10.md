---
description: ''
layout: schema
name: Data10
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
- description: ''
  name: requiredFields
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data10-schema.json
slug: zoominfo-data10
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"personid\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              }\n            },\n            \"required\": [\n              \"personid\"\n            ]\n          },\n          \"data\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n              \
  \  \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"firstName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"middleName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"lastName\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"email\": {\n                  \"type\": \"string\",\n                  \"example\": \"jsmith@example.com\"\n                },\n                \"hasCanadianEmail\": {\n                  \"type\": \"string\",\n                  \"example\": \"jsmith@example.com\"\n                },\n                \"phone\": {\n                  \"type\": \"string\",\n                  \"example\": \"+1-555-555-1234\"\n              \
  \  },\n                \"street\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"city\": {\n                  \"type\": \"string\",\n                  \"example\": \"San Francisco\"\n                },\n                \"region\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"company\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"id\",\n                \"firstName\",\n                \"middleName\",\n                \"lastName\",\n                \"email\",\n                \"hasCanadianEmail\",\n\
  \                \"phone\",\n                \"street\",\n                \"city\",\n                \"region\",\n                \"company\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n        ]\n      }\n    },\n    \"requiredFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\",\n    \"requiredFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data10-schema.json
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
title: Data10
---
