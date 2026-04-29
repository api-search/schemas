---
description: ''
layout: schema
name: Result8
properties_list:
- description: ''
  name: input
  type: object
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-result8-schema.json
slug: zoominfo-result8
source_filename: zoominfo-result8-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"input\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"companyname\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        }\n      },\n      \"required\": [\n        \"companyname\"\n      ]\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"ticker\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"domainList\": {\n        \
  \    \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"logo\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"socialMediaUrls\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": \"https://www.example.com\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"standard\"\n                },\n                \"url\": {\n                  \"type\": \"string\",\n                  \"example\": \"https://www.example.com/resource\"\n                },\n                \"followerCount\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n   \
  \           },\n              \"required\": [\n                \"type\",\n                \"url\",\n                \"followerCount\"\n              ]\n            }\n          },\n          \"revenue\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"employeeCount\": {\n            \"type\": \"integer\",\n            \"example\": 250\n          },\n          \"numberOfContactsInZoomInfo\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"phone\": {\n            \"type\": \"string\",\n            \"example\": \"+1-555-555-1234\"\n          },\n          \"fax\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"street\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"city\": {\n            \"type\": \"string\",\n            \"example\": \"San Francisco\"\n          },\n       \
  \   \"state\": {\n            \"type\": \"string\",\n            \"example\": \"CA\"\n          },\n          \"zipCode\": {\n            \"type\": \"string\",\n            \"example\": \"94105\"\n          },\n          \"country\": {\n            \"type\": \"string\",\n            \"example\": \"US\"\n          },\n          \"continent\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"companyStatus\": {\n            \"type\": \"string\",\n            \"example\": \"active\"\n          },\n          \"companyStatusDate\": {\n            \"type\": \"string\",\n            \"example\": \"active\"\n          },\n          \"employeeGrowth\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"oneYearGrowthRate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"twoYearGrowthRate\": {\n                \"type\": \"string\"\
  ,\n                \"example\": \"example_value\"\n              },\n              \"employeeGrowthDataPoints\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\"\n                }\n              }\n            },\n            \"required\": [\n              \"oneYearGrowthRate\",\n              \"twoYearGrowthRate\",\n              \"employeeGrowthDataPoints\"\n            ]\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"ticker\",\n          \"name\",\n          \"website\",\n          \"domainList\",\n          \"logo\",\n          \"socialMediaUrls\",\n          \"revenue\",\n          \"employeeCount\",\n          \"numberOfContactsInZoomInfo\",\n          \"phone\",\n          \"fax\",\n          \"street\"\
  ,\n          \"city\",\n          \"state\",\n          \"zipCode\",\n          \"country\",\n          \"continent\",\n          \"companyStatus\",\n          \"companyStatusDate\",\n          \"employeeGrowth\",\n          \"type\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"input\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result8\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-result8-schema.json
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
title: Result8
---
