---
description: SharedCompany schema from Avalara API
layout: schema
name: SharedCompany
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: companyCode
  type: string
- description: Tax identification number
  name: taxPayerId
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: phoneNumber
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: isActive
  type: boolean
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/shared-company-service-shared-company-schema.json
slug: shared-company-service-shared-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-shared-company-schema.json\",\n  \"title\": \"SharedCompany\",\n  \"description\": \"SharedCompany schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\"\n    },\n    \"taxPayerId\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"line2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n      \
  \  },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-shared-company-schema.json
tags:
- Taxes
title: SharedCompany
---
