---
description: ''
layout: schema
name: Data14
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data14-schema.json
slug: zoominfo-data14
source_filename: zoominfo-data14-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"companycity\": {\n                \"type\": \"string\",\n                \"example\": \"San Francisco\"\n              },\n              \"companyname\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"companystate\": {\n                \"type\": \"string\",\n                \"example\": \"CA\"\n              },\n              \"companystreet\": {\n              \
  \  \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"companywebsite\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"companycity\",\n              \"companyname\",\n              \"companystate\",\n              \"companystreet\",\n              \"companywebsite\"\n            ]\n          },\n          \"data\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"locationMatch\": {\n\
  \                  \"type\": \"object\",\n                  \"properties\": {\n                    \"companyId\": {\n                      \"type\": \"object\"\n                    },\n                    \"address\": {\n                      \"type\": \"object\"\n                    },\n                    \"addressStatus\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"companyId\",\n                    \"address\",\n                    \"addressStatus\"\n                  ]\n                },\n                \"website\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"state\": {\n                  \"type\": \"string\",\n                  \"example\": \"CA\"\n                },\n                \"city\": {\n                  \"type\": \"string\",\n                  \"example\": \"San Francisco\"\n \
  \               }\n              },\n              \"required\": [\n                \"id\",\n                \"name\",\n                \"locationMatch\",\n                \"website\",\n                \"state\",\n                \"city\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data14\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data14-schema.json
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
title: Data14
---
