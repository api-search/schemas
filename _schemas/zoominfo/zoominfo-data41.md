---
description: ''
layout: schema
name: Data41
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data41-schema.json
slug: zoominfo-data41
source_filename: zoominfo-data41-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"data\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"geoLocation\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"location_long\": {\n                    \"type\": \"number\",\n                    \"example\": 75.5\n                \
  \  },\n                  \"location_lat\": {\n                    \"type\": \"number\",\n                    \"example\": 75.5\n                  },\n                  \"country_code\": {\n                    \"type\": \"string\",\n                    \"example\": \"US\"\n                  },\n                  \"province\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"location_long\",\n                  \"location_lat\",\n                  \"country_code\",\n                  \"province\"\n                ]\n              },\n              \"ispInfo\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"domain\": {\n                    \"type\": \"string\",\n                    \"example\": \"example.com\"\n                  },\n                  \"ip_hi_string\": {\n                    \"type\"\
  : \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"ip_lo_string\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"example\": \"standard\"\n                  }\n                },\n                \"required\": [\n                  \"domain\",\n                  \"ip_hi_string\",\n                  \"ip_lo_string\",\n                  \"name\",\n                  \"type\"\n                ]\n              }\n            },\n            \"required\": [\n              \"geoLocation\",\n              \"ispInfo\"\n            ]\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n\
  \        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data41\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data41-schema.json
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
title: Data41
---
