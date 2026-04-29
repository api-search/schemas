---
description: ''
layout: schema
name: Enrichcontactsusingrequiredfields
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-enrichcontactsusingrequiredfields-schema.json
slug: zoominfo-enrichcontactsusingrequiredfields
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"personid\": {\n                    \"type\": \"integer\",\n                    \"example\": 500123\n                  }\n                },\n                \"required\": [\n                  \"personid\"\n\
  \                ]\n              },\n              \"data\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": {\n                      \"type\": \"object\"\n                    },\n                    \"firstName\": {\n                      \"type\": \"object\"\n                    },\n                    \"middleName\": {\n                      \"type\": \"object\"\n                    },\n                    \"lastName\": {\n                      \"type\": \"object\"\n                    },\n                    \"email\": {\n                      \"type\": \"object\"\n                    },\n                    \"hasCanadianEmail\": {\n                      \"type\": \"object\"\n                    },\n                    \"phone\": {\n                      \"type\": \"object\"\n    \
  \                },\n                    \"street\": {\n                      \"type\": \"object\"\n                    },\n                    \"city\": {\n                      \"type\": \"object\"\n                    },\n                    \"region\": {\n                      \"type\": \"object\"\n                    },\n                    \"company\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"id\",\n                    \"firstName\",\n                    \"middleName\",\n                    \"lastName\",\n                    \"email\",\n                    \"hasCanadianEmail\",\n                    \"phone\",\n                    \"street\",\n                    \"city\",\n                    \"region\",\n                    \"company\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"input\",\n         \
  \     \"data\"\n            ]\n          }\n        },\n        \"requiredFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\",\n        \"requiredFields\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichcontactsusingrequiredfields\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichcontactsusingrequiredfields-schema.json
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
title: Enrichcontactsusingrequiredfields
---
