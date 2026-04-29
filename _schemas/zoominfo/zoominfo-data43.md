---
description: ''
layout: schema
name: Data43
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data43-schema.json
slug: zoominfo-data43
source_filename: zoominfo-data43-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"data\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"company\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"city\": {\n                    \"type\": \"string\",\n                    \"example\": \"San Francisco\"\n                \
  \  },\n                  \"country\": {\n                    \"type\": \"string\",\n                    \"example\": \"US\"\n                  },\n                  \"employeeCount\": {\n                    \"type\": \"integer\",\n                    \"example\": 250\n                  },\n                  \"id\": {\n                    \"type\": \"integer\",\n                    \"example\": 500123\n                  },\n                  \"industries\": {\n                    \"type\": \"array\",\n                    \"description\": \"\",\n                    \"example\": [],\n                    \"items\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  },\n                  \"revenue\": {\n                    \"type\": \"integer\",\n                    \"example\": 100\n                  },\n\
  \                  \"state\": {\n                    \"type\": \"string\",\n                    \"example\": \"CA\"\n                  },\n                  \"street\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"ticker\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"website\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"zipCode\": {\n                    \"type\": \"string\",\n                    \"example\": \"94105\"\n                  }\n                },\n                \"required\": [\n                  \"city\",\n                  \"country\",\n                  \"employeeCount\",\n                  \"id\",\n                  \"industries\",\n                  \"name\",\n                  \"revenue\"\
  ,\n                  \"state\",\n                  \"street\",\n                  \"ticker\",\n                  \"website\",\n                  \"zipCode\"\n                ]\n              },\n              \"geoLocation\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"location_long\": {\n                    \"type\": \"number\",\n                    \"example\": 75.5\n                  },\n                  \"location_lat\": {\n                    \"type\": \"number\",\n                    \"example\": 75.5\n                  },\n                  \"country_code\": {\n                    \"type\": \"string\",\n                    \"example\": \"US\"\n                  },\n                  \"province\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"location_long\",\n                  \"location_lat\"\
  ,\n                  \"country_code\",\n                  \"province\"\n                ]\n              }\n            },\n            \"required\": [\n              \"company\",\n              \"geoLocation\"\n            ]\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data43\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data43-schema.json
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
title: Data43
---
