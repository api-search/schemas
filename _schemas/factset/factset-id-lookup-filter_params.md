---
description: The filters parameter (if used) must contain one or both of theinlcude and exclude filters
layout: schema
name: filter_params
properties_list:
- description: This parameter filter objects to be included in the results
  name: include
  type: array
- description: This parameter filter objects to be excluded from the results
  name: exclude
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-id-lookup-filter_params-schema.json
slug: factset-id-lookup-filter_params
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"filter_params\",\n  \"type\": \"object\",\n  \"description\": \"The filters parameter (if used) must contain one or both of theinlcude and exclude filters\\n\",\n  \"properties\": {\n    \"include\": {\n      \"type\": \"array\",\n      \"description\": \"This parameter filter objects to be included in the results\"\n    },\n    \"exclude\": {\n      \"type\": \"array\",\n      \"description\": \"This parameter filter objects to be excluded from the results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-id-lookup-filter_params-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: filter_params
---
