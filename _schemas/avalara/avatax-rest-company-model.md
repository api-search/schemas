---
description: CompanyModel schema from Avalara API
layout: schema
name: CompanyModel
properties_list:
- description: Unique identifier for the company
  name: id
  type: integer
- description: Short code identifying this company
  name: companyCode
  type: string
- description: Display name of the company
  name: name
  type: string
- description: Whether this is the default company for the account
  name: isDefault
  type: boolean
- description: ''
  name: isActive
  type: boolean
- description: Tax identification number (EIN, TIN)
  name: taxpayerIdNumber
  type: string
- description: ''
  name: hasProfile
  type: boolean
- description: ''
  name: isReportingEntity
  type: boolean
- description: Default country for this company
  name: defaultCountry
  type: string
- description: Default currency code
  name: baseCurrencyCode
  type: string
- description: ''
  name: sstEffDate
  type: string
- description: ''
  name: roundingLevelId
  type: string
- description: ''
  name: sstPId
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-company-model-schema.json
slug: avatax-rest-company-model
source_filename: avatax-rest-company-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-company-model-schema.json\",\n  \"title\": \"CompanyModel\",\n  \"description\": \"CompanyModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the company\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Short code identifying this company\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the company\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default company for the account\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\"\n    },\n    \"taxpayerIdNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification\
  \ number (EIN, TIN)\"\n    },\n    \"hasProfile\": {\n      \"type\": \"boolean\"\n    },\n    \"isReportingEntity\": {\n      \"type\": \"boolean\"\n    },\n    \"defaultCountry\": {\n      \"type\": \"string\",\n      \"description\": \"Default country for this company\"\n    },\n    \"baseCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Default currency code\"\n    },\n    \"sstEffDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"roundingLevelId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Line\",\n        \"Document\"\n      ]\n    },\n    \"sstPId\": {\n      \"type\": \"string\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-company-model-schema.json
tags:
- Taxes
title: CompanyModel
---
