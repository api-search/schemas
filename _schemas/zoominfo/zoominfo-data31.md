---
description: ''
layout: schema
name: Data31
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data31-schema.json
slug: zoominfo-data31
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"companyname\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"companyid\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              }\n            }\n          },\n          \"data\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"\
  type\": \"object\",\n              \"properties\": {\n                \"parentage\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"familyTree\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"companyId\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                }\n              },\n              \"required\": [\n                \"parentage\",\n                \"familyTree\",\n                \"companyId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n       \
  \ ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data31\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data31-schema.json
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
title: Data31
---
