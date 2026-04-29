---
description: ''
layout: schema
name: Enrichcorporatehierarchy-multiplecompanies
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-enrichcorporatehierarchy-multiplecompanies-schema.json
slug: zoominfo-enrichcorporatehierarchy-multiplecompanies
source_filename: zoominfo-enrichcorporatehierarchy-multiplecompanies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"outputFields\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"result\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"input\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"companyname\": {\n                    \"type\": \"string\",\n                    \"example\": \"Acme Corporation\"\n                  },\n                  \"companyid\": {\n                    \"type\": \"\
  integer\",\n                    \"example\": 500123\n                  }\n                }\n              },\n              \"data\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"parentage\": {\n                      \"type\": \"object\"\n                    },\n                    \"familyTree\": {\n                      \"type\": \"object\"\n                    },\n                    \"companyId\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"parentage\",\n                    \"familyTree\",\n                    \"companyId\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"input\",\n              \"data\"\n      \
  \      ]\n          }\n        }\n      },\n      \"required\": [\n        \"outputFields\",\n        \"result\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichcorporatehierarchy-multiplecompanies\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichcorporatehierarchy-multiplecompanies-schema.json
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
title: Enrichcorporatehierarchy-multiplecompanies
---
