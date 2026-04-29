---
description: ''
layout: schema
name: Company15
properties_list:
- description: ''
  name: division
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: descriptionList
  type: array
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
  name: logo
  type: string
- description: ''
  name: sicCodes
  type: array
- description: ''
  name: naicsCodes
  type: array
- description: ''
  name: website
  type: string
- description: ''
  name: revenue
  type: string
- description: ''
  name: revenueNumeric
  type: integer
- description: ''
  name: employeeCount
  type: integer
- description: ''
  name: type
  type: string
- description: ''
  name: ticker
  type: string
- description: ''
  name: ranking
  type: array
- description: ''
  name: socialMediaUrls
  type: array
- description: ''
  name: primaryIndustry
  type: array
- description: ''
  name: industries
  type: array
- description: ''
  name: revenueRange
  type: string
- description: ''
  name: employeeRange
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company15-schema.json
slug: zoominfo-company15
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"division\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"descriptionList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          }\n        },\n        \"required\": [\n          \"description\"\n        ]\n      }\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"continent\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sicCodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          }\n        },\n        \"required\"\
  : [\n          \"id\",\n          \"name\"\n        ]\n      }\n    },\n    \"naicsCodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\"\n        ]\n      }\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"revenue\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"revenueNumeric\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"employeeCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"type\": {\n      \"type\": \"string\",\n  \
  \    \"example\": \"standard\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"ranking\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"socialMediaUrls\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"primaryIndustry\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"industries\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"revenueRange\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"employeeRange\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"division\",\n    \"id\",\n    \"name\",\n    \"descriptionList\",\n    \"phone\",\n    \"fax\",\n    \"street\",\n    \"city\",\n    \"state\",\n    \"zipCode\",\n    \"country\",\n    \"continent\",\n    \"logo\",\n    \"sicCodes\",\n    \"naicsCodes\",\n    \"website\",\n    \"revenue\",\n    \"revenueNumeric\",\n    \"employeeCount\",\n    \"type\",\n    \"ticker\",\n    \"ranking\",\n    \"socialMediaUrls\",\n    \"primaryIndustry\",\n    \"industries\",\n    \"revenueRange\",\n    \"employeeRange\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Company15\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company15-schema.json
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
title: Company15
---
