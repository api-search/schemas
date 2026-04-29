---
description: ''
layout: schema
name: Datum
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: firstName
  type: string
- description: ''
  name: middleName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: validDate
  type: string
- description: ''
  name: lastUpdatedDate
  type: string
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: contactAccuracyScore
  type: integer
- description: ''
  name: hasEmail
  type: boolean
- description: ''
  name: hasSupplementalEmail
  type: boolean
- description: ''
  name: hasDirectPhone
  type: boolean
- description: ''
  name: hasMobilePhone
  type: boolean
- description: ''
  name: hasCompanyIndustry
  type: boolean
- description: ''
  name: hasCompanyPhone
  type: boolean
- description: ''
  name: hasCompanyStreet
  type: boolean
- description: ''
  name: hasCompanyState
  type: boolean
- description: ''
  name: hasCompanyZipCode
  type: boolean
- description: ''
  name: hasCompanyCountry
  type: boolean
- description: ''
  name: hasCompanyRevenue
  type: boolean
- description: ''
  name: hasCompanyEmployeeCount
  type: boolean
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-datum-schema.json
slug: zoominfo-datum
source_filename: zoominfo-datum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"validDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"contactAccuracyScore\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"hasEmail\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasSupplementalEmail\": {\n      \"type\": \"boolean\"\
  ,\n      \"example\": true\n    },\n    \"hasDirectPhone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasMobilePhone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyIndustry\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyPhone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyStreet\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyState\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyZipCode\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyCountry\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyRevenue\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasCompanyEmployeeCount\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"company\": {\n      \"type\": \"\
  object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"firstName\",\n    \"middleName\",\n    \"lastName\",\n    \"validDate\",\n    \"lastUpdatedDate\",\n    \"jobTitle\",\n    \"contactAccuracyScore\",\n    \"hasEmail\",\n    \"hasSupplementalEmail\",\n    \"hasDirectPhone\",\n    \"hasMobilePhone\",\n    \"hasCompanyIndustry\",\n    \"hasCompanyPhone\",\n    \"hasCompanyStreet\",\n    \"hasCompanyState\",\n    \"hasCompanyZipCode\",\n    \"hasCompanyCountry\",\n    \"hasCompanyRevenue\",\n    \"hasCompanyEmployeeCount\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datum\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-datum-schema.json
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
title: Datum
---
