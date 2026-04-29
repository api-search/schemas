---
description: ''
layout: schema
name: Result17
properties_list:
- description: ''
  name: input
  type: array
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-result17-schema.json
slug: zoominfo-result17
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"geoLocation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"location_long\": {\n              \"type\": \"number\",\n              \"example\": 75.5\n            },\n            \"location_lat\": {\n              \"type\": \"number\",\n              \"example\": 75.5\n            },\n            \"country_code\": {\n              \"type\": \"string\",\n              \"example\": \"US\"\n            },\n            \"province\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"location_long\",\n            \"location_lat\",\n            \"country_code\"\
  ,\n            \"province\"\n          ]\n        },\n        \"ispInfo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"domain\": {\n              \"type\": \"string\",\n              \"example\": \"example.com\"\n            },\n            \"ip_hi_string\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"ip_lo_string\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"example\": \"Acme Corporation\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"standard\"\n            }\n          },\n          \"required\": [\n            \"domain\",\n            \"ip_hi_string\",\n            \"ip_lo_string\",\n            \"name\",\n            \"type\"\n          ]\n        }\n      },\n      \"required\":\
  \ [\n        \"geoLocation\",\n        \"ispInfo\"\n      ]\n    }\n  },\n  \"required\": [\n    \"input\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result17\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-result17-schema.json
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
title: Result17
---
