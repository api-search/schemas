---
description: ''
layout: schema
name: IPbelongstoacompany
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-i-pbelongstoacompany-schema.json
slug: zoominfo-i-pbelongstoacompany
source_filename: zoominfo-i-pbelongstoacompany-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              },\n              \"data\": {\n                \"type\": \"object\",\n               \
  \ \"properties\": {\n                  \"company\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"city\": {\n                        \"type\": \"object\"\n                      },\n                      \"country\": {\n                        \"type\": \"object\"\n                      },\n                      \"employeeCount\": {\n                        \"type\": \"object\"\n                      },\n                      \"id\": {\n                        \"type\": \"object\"\n                      },\n                      \"industries\": {\n                        \"type\": \"object\"\n                      },\n                      \"name\": {\n                        \"type\": \"object\"\n                      },\n                      \"revenue\": {\n                        \"type\": \"object\"\n                      },\n                      \"state\": {\n                        \"type\": \"object\"\n            \
  \          },\n                      \"street\": {\n                        \"type\": \"object\"\n                      },\n                      \"ticker\": {\n                        \"type\": \"object\"\n                      },\n                      \"website\": {\n                        \"type\": \"object\"\n                      },\n                      \"zipCode\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"city\",\n                      \"country\",\n                      \"employeeCount\",\n                      \"id\",\n                      \"industries\",\n                      \"name\",\n                      \"revenue\",\n                      \"state\",\n                      \"street\",\n                      \"ticker\",\n                      \"website\",\n                      \"zipCode\"\n                    ]\n                  },\n                \
  \  \"geoLocation\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"location_long\": {\n                        \"type\": \"object\"\n                      },\n                      \"location_lat\": {\n                        \"type\": \"object\"\n                      },\n                      \"country_code\": {\n                        \"type\": \"object\"\n                      },\n                      \"province\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"location_long\",\n                      \"location_lat\",\n                      \"country_code\",\n                      \"province\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"company\",\n                  \"geoLocation\"\n                ]\n              }\n            },\n \
  \           \"required\": [\n              \"input\",\n              \"data\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPbelongstoacompany\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-i-pbelongstoacompany-schema.json
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
title: IPbelongstoacompany
---
