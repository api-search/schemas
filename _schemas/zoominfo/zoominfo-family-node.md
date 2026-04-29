---
description: ''
layout: schema
name: FamilyNode
properties_list:
- description: ''
  name: companyId
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: subUnitTypeInfo
  type: object
- description: ''
  name: familyNodes
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-family-node-schema.json
slug: zoominfo-family-node
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"subUnitTypeInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"typeId\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"typeDescription\": {\n          \"type\": \"string\",\n          \"example\": \"Enterprise software company\"\n        }\n      },\n      \"required\": [\n        \"typeId\",\n        \"typeDescription\"\n      ]\n    },\n    \"familyNodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"companyId\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"city\": {\n            \"type\": \"string\",\n            \"example\": \"San Francisco\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"example\": \"CA\"\n          },\n          \"subUnitTypeInfo\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"typeId\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"typeDescription\": {\n                \"type\": \"string\",\n                \"example\": \"Enterprise software company\"\n              }\n            },\n            \"required\": [\n              \"typeId\",\n              \"typeDescription\"\n            ]\n          },\n          \"familyNodes\":\
  \ {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"companyId\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"city\": {\n                  \"type\": \"string\",\n                  \"example\": \"San Francisco\"\n                },\n                \"state\": {\n                  \"type\": \"string\",\n                  \"example\": \"CA\"\n                },\n                \"subUnitTypeInfo\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"typeId\": {\n                      \"type\": \"object\"\n                    },\n                    \"typeDescription\"\
  : {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"typeId\",\n                    \"typeDescription\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"companyId\",\n                \"name\",\n                \"city\",\n                \"state\",\n                \"subUnitTypeInfo\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"companyId\",\n          \"name\",\n          \"city\",\n          \"state\",\n          \"subUnitTypeInfo\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"companyId\",\n    \"name\",\n    \"city\",\n    \"state\",\n    \"subUnitTypeInfo\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FamilyNode\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-family-node-schema.json
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
title: FamilyNode
---
