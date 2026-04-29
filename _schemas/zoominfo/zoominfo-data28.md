---
description: ''
layout: schema
name: Data28
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data28-schema.json
slug: zoominfo-data28
source_filename: zoominfo-data28-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"statusCode\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"input\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"zi_c_location_id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"address\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"zi_c_country\": {\n                    \"type\": \"string\",\n                    \"example\": \"US\"\n                  },\n   \
  \               \"zi_c_state\": {\n                    \"type\": \"string\",\n                    \"example\": \"CA\"\n                  }\n                },\n                \"required\": [\n                  \"zi_c_country\",\n                  \"zi_c_state\"\n                ]\n              },\n              \"zi_c_url\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com/resource\"\n              },\n              \"phone\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"zi_c_country\": {\n                    \"type\": \"string\",\n                    \"example\": \"US\"\n                  },\n                  \"zi_c_phone\": {\n                    \"type\": \"string\",\n                    \"example\": \"+1-555-555-1234\"\n                  }\n                },\n                \"required\": [\n                  \"zi_c_country\",\n                  \"zi_c_phone\"\n                ]\n\
  \              }\n            }\n          },\n          \"data\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"zi_c_location_id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"zi_es_ecid\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"zi_es_location_id\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"zi_c_is_hq\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"zi_c_company_name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"zi_c_tier_grade\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"zi_c_name\": {\n  \
  \              \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"zi_c_name_display\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"zi_c_url\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com/resource\"\n              },\n              \"zi_c_street\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"zi_c_city\": {\n                \"type\": \"string\",\n                \"example\": \"San Francisco\"\n              },\n              \"zi_c_state\": {\n                \"type\": \"string\",\n                \"example\": \"CA\"\n              },\n              \"zi_c_zip\": {\n                \"type\": \"string\",\n                \"example\": \"94105\"\n              },\n              \"zi_c_country\": {\n                \"type\"\
  : \"string\",\n                \"example\": \"US\"\n              },\n              \"zi_c_legal_entity_type\": {\n                \"type\": \"string\",\n                \"example\": \"standard\"\n              },\n              \"zi_c_street_2\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"zi_c_location_id\",\n              \"zi_es_ecid\",\n              \"zi_es_location_id\",\n              \"zi_c_is_hq\",\n              \"zi_c_company_name\",\n              \"zi_c_tier_grade\",\n              \"zi_c_name\",\n              \"zi_c_name_display\",\n              \"zi_c_url\",\n              \"zi_c_street\",\n              \"zi_c_city\",\n              \"zi_c_state\",\n              \"zi_c_zip\",\n              \"zi_c_country\"\n            ]\n          }\n        },\n        \"required\": [\n          \"statusCode\",\n          \"input\",\n          \"data\"\n   \
  \     ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data28\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data28-schema.json
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
title: Data28
---
