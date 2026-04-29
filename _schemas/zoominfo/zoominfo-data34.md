---
description: ''
layout: schema
name: Data34
properties_list:
- description: ''
  name: parentage
  type: array
- description: ''
  name: familyTree
  type: array
- description: ''
  name: companyId
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data34-schema.json
slug: zoominfo-data34
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"parentage\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"familyTree\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"companyId\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"city\": {\n            \"type\": \"string\",\n            \"example\": \"San Francisco\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"example\": \"CA\"\n          },\n          \"familyNodes\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n  \
  \          \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"companyId\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"city\": {\n                  \"type\": \"string\",\n                  \"example\": \"San Francisco\"\n                },\n                \"state\": {\n                  \"type\": \"string\",\n                  \"example\": \"CA\"\n                },\n                \"subUnitTypeInfo\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"typeId\": {\n                      \"type\": \"object\"\n                    },\n                    \"typeDescription\": {\n                      \"type\": \"object\"\n                    }\n                  },\n  \
  \                \"required\": [\n                    \"typeId\",\n                    \"typeDescription\"\n                  ]\n                },\n                \"familyNodes\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"companyId\",\n                \"name\",\n                \"city\",\n                \"state\",\n                \"subUnitTypeInfo\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"companyId\",\n          \"name\",\n          \"city\",\n          \"state\",\n          \"familyNodes\"\n        ]\n      }\n    },\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    }\n  },\n  \"required\": [\n    \"parentage\",\n    \"familyTree\",\n   \
  \ \"companyId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data34\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data34-schema.json
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
title: Data34
---
