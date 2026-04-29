---
description: CompanyData schema from Avalara API
layout: schema
name: CompanyData
properties_list:
- description: Business class (0=ILEC, 1=CLEC, etc.)
  name: bscl
  type: integer
- description: Service class (0=Primary Local, 1=Primary Long Distance)
  name: svcl
  type: integer
- description: Facilities-based indicator
  name: fclt
  type: boolean
- description: Franchise indicator
  name: frch
  type: boolean
- description: Regulated indicator
  name: reg
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-company-data-schema.json
slug: communications-company-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-company-data-schema.json\",\n  \"title\": \"CompanyData\",\n  \"description\": \"CompanyData schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bscl\": {\n      \"type\": \"integer\",\n      \"description\": \"Business class (0=ILEC, 1=CLEC, etc.)\"\n    },\n    \"svcl\": {\n      \"type\": \"integer\",\n      \"description\": \"Service class (0=Primary Local, 1=Primary Long Distance)\"\n    },\n    \"fclt\": {\n      \"type\": \"boolean\",\n      \"description\": \"Facilities-based indicator\"\n    },\n    \"frch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Franchise indicator\"\n    },\n    \"reg\": {\n      \"type\": \"boolean\",\n      \"description\": \"Regulated indicator\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-company-data-schema.json
tags:
- Taxes
title: CompanyData
---
