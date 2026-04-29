---
description: ''
layout: schema
name: Data16
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: result
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data16-schema.json
slug: zoominfo-data16
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"companyname\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              }\n            },\n            \"required\": [\n              \"companyname\"\n            ]\n          },\n          \"data\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\"\
  : {\n                \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"ticker\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                },\n                \"website\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"domainList\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"logo\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"socialMediaUrls\"\
  : {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": \"https://www.example.com\",\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"revenue\": {\n                  \"type\": \"integer\",\n                  \"example\": 100\n                },\n                \"employeeCount\": {\n                  \"type\": \"integer\",\n                  \"example\": 250\n                },\n                \"numberOfContactsInZoomInfo\": {\n                  \"type\": \"integer\",\n                  \"example\": 100\n                },\n                \"phone\": {\n                  \"type\": \"string\",\n                  \"example\": \"+1-555-555-1234\"\n                },\n                \"fax\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"street\": {\n        \
  \          \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"city\": {\n                  \"type\": \"string\",\n                  \"example\": \"San Francisco\"\n                },\n                \"state\": {\n                  \"type\": \"string\",\n                  \"example\": \"CA\"\n                },\n                \"zipCode\": {\n                  \"type\": \"string\",\n                  \"example\": \"94105\"\n                },\n                \"country\": {\n                  \"type\": \"string\",\n                  \"example\": \"US\"\n                },\n                \"continent\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"companyStatus\": {\n                  \"type\": \"string\",\n                  \"example\": \"active\"\n                },\n                \"companyStatusDate\": {\n                  \"type\": \"\
  string\",\n                  \"example\": \"active\"\n                },\n                \"employeeGrowth\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"oneYearGrowthRate\": {\n                      \"type\": \"object\"\n                    },\n                    \"twoYearGrowthRate\": {\n                      \"type\": \"object\"\n                    },\n                    \"employeeGrowthDataPoints\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"oneYearGrowthRate\",\n                    \"twoYearGrowthRate\",\n                    \"employeeGrowthDataPoints\"\n                  ]\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"standard\"\n                }\n              },\n              \"required\": [\n                \"id\",\n                \"\
  ticker\",\n                \"name\",\n                \"website\",\n                \"domainList\",\n                \"logo\",\n                \"socialMediaUrls\",\n                \"revenue\",\n                \"employeeCount\",\n                \"numberOfContactsInZoomInfo\",\n                \"phone\",\n                \"fax\",\n                \"street\",\n                \"city\",\n                \"state\",\n                \"zipCode\",\n                \"country\",\n                \"continent\",\n                \"companyStatus\",\n                \"companyStatusDate\",\n                \"employeeGrowth\",\n                \"type\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"input\",\n          \"data\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"result\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data16\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data16-schema.json
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
title: Data16
---
