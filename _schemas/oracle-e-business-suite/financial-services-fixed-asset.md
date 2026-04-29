---
description: ''
layout: schema
name: FixedAsset
properties_list:
- description: Asset identifier
  name: assetId
  type: integer
- description: Asset number
  name: assetNumber
  type: string
- description: Asset description
  name: assetDescription
  type: string
- description: Asset category identifier
  name: assetCategoryId
  type: integer
- description: Asset type
  name: assetType
  type: string
- description: Serial number
  name: serialNumber
  type: string
- description: Tag number
  name: tagNumber
  type: string
- description: ''
  name: dateEffective
  type: string
- description: Date placed in service
  name: dateInService
  type: string
- description: Asset cost
  name: cost
  type: number
- description: Salvage value
  name: salvageValue
  type: number
- description: Depreciation method
  name: depreciationMethod
  type: string
- description: Useful life in months
  name: lifeInMonths
  type: integer
- description: Book type code (corporate or tax)
  name: bookTypeCode
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-fixed-asset-schema.json
slug: financial-services-fixed-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FixedAsset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"type\": \"integer\",\n      \"description\": \"Asset identifier\"\n    },\n    \"assetNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Asset number\"\n    },\n    \"assetDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Asset description\"\n    },\n    \"assetCategoryId\": {\n      \"type\": \"integer\",\n      \"description\": \"Asset category identifier\"\n    },\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"Asset type\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number\"\n    },\n    \"tagNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Tag number\"\n    },\n    \"dateEffective\": {\n      \"type\": \"string\"\n    },\n    \"dateInService\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Date placed in service\"\n    },\n    \"cost\": {\n      \"type\": \"number\",\n      \"description\": \"Asset cost\"\n    },\n    \"salvageValue\": {\n      \"type\": \"number\",\n      \"description\": \"Salvage value\"\n    },\n    \"depreciationMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Depreciation method\"\n    },\n    \"lifeInMonths\": {\n      \"type\": \"integer\",\n      \"description\": \"Useful life in months\"\n    },\n    \"bookTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Book type code (corporate or tax)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-fixed-asset-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: FixedAsset
---
