---
description: ''
layout: schema
name: MatchbyZoomInfocompanyID1
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-matchby-zoom-infocompany-id1-schema.json
slug: zoominfo-matchby-zoom-infocompany-id1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"statusCode\": {\n                \"type\": \"integer\",\n                \"example\": 100\n              },\n              \"input\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"zi_c_id\": {\n                    \"type\": \"integer\",\n                    \"example\": 500123\n                  }\n    \
  \            },\n                \"required\": [\n                  \"zi_c_id\"\n                ]\n              },\n              \"data\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"errorMessage\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"errorMessage\"\n                ]\n              }\n            },\n            \"required\": [\n              \"statusCode\",\n              \"input\",\n              \"data\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MatchbyZoomInfocompanyID1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-matchby-zoom-infocompany-id1-schema.json
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
title: MatchbyZoomInfocompanyID1
---
