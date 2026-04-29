---
description: ''
layout: schema
name: Data17
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: ticker
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: website
  type: string
- description: ''
  name: domainList
  type: array
- description: ''
  name: logo
  type: string
- description: ''
  name: socialMediaUrls
  type: array
- description: ''
  name: revenue
  type: integer
- description: ''
  name: employeeCount
  type: integer
- description: ''
  name: numberOfContactsInZoomInfo
  type: integer
- description: ''
  name: phone
  type: string
- description: ''
  name: fax
  type: string
- description: ''
  name: street
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zipCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: continent
  type: string
- description: ''
  name: companyStatus
  type: string
- description: ''
  name: companyStatusDate
  type: string
- description: ''
  name: employeeGrowth
  type: object
- description: ''
  name: type
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data17-schema.json
slug: zoominfo-data17
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"domainList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"socialMediaUrls\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n\
  \          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          },\n          \"followerCount\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"url\",\n          \"followerCount\"\n        ]\n      }\n    },\n    \"revenue\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"employeeCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"numberOfContactsInZoomInfo\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"continent\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"companyStatus\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"companyStatusDate\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"employeeGrowth\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"oneYearGrowthRate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"twoYearGrowthRate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"employeeGrowthDataPoints\": {\n          \"type\": \"array\",\n          \"\
  description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      },\n      \"required\": [\n        \"oneYearGrowthRate\",\n        \"twoYearGrowthRate\",\n        \"employeeGrowthDataPoints\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"ticker\",\n    \"name\",\n    \"website\",\n    \"domainList\",\n    \"logo\",\n    \"socialMediaUrls\",\n    \"revenue\",\n    \"employeeCount\",\n    \"numberOfContactsInZoomInfo\",\n    \"phone\",\n    \"fax\",\n    \"street\",\n    \"city\",\n    \"state\",\n    \"zipCode\",\n    \"country\",\n    \"continent\",\n    \"companyStatus\",\n    \"companyStatusDate\",\n    \"employeeGrowth\",\n    \"type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data17\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data17-schema.json
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
title: Data17
---
