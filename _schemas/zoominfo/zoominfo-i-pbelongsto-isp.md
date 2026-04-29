---
description: ''
layout: schema
name: IPbelongstoISP
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-i-pbelongsto-isp-schema.json
slug: zoominfo-i-pbelongsto-isp
source_filename: zoominfo-i-pbelongsto-isp-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"data\": {\n                \"type\": \"object\",\n               \
  \ \"properties\": {\n                  \"geoLocation\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"location_long\": {\n                        \"type\": \"object\"\n                      },\n                      \"location_lat\": {\n                        \"type\": \"object\"\n                      },\n                      \"country_code\": {\n                        \"type\": \"object\"\n                      },\n                      \"province\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"location_long\",\n                      \"location_lat\",\n                      \"country_code\",\n                      \"province\"\n                    ]\n                  },\n                  \"ispInfo\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                    \
  \  \"domain\": {\n                        \"type\": \"object\"\n                      },\n                      \"ip_hi_string\": {\n                        \"type\": \"object\"\n                      },\n                      \"ip_lo_string\": {\n                        \"type\": \"object\"\n                      },\n                      \"name\": {\n                        \"type\": \"object\"\n                      },\n                      \"type\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"domain\",\n                      \"ip_hi_string\",\n                      \"ip_lo_string\",\n                      \"name\",\n                      \"type\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"geoLocation\",\n                  \"ispInfo\"\n                ]\n              }\n            },\n       \
  \     \"required\": [\n              \"input\",\n              \"data\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPbelongstoISP\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-i-pbelongsto-isp-schema.json
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
title: IPbelongstoISP
---
