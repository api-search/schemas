---
description: Data model returned when the parameter **flatten=Y** is used in the request. This flattened, simplified JSON data returned from **flatten=Y** can be conceptualized as a table (rows and columns) where each data object in the result is a row in the table and the field names are the column names. There will be one data object for each request containing the request, fsymId if requested, and Key-Value pairs for each data item (formula).
layout: schema
name: cross_sectional_result_object_flattened
properties_list:
- description: Identifier requested.
  name: requestId
  type: string
- description: 'The **fsymId** field returned is the FactSet Default Permanent Identifier for the `requestId`. For all supported `requestId` symbol types, the `fsymId` parameter will return the Regional Level PermId '
  name: fsymId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-formula-cross_sectional_result_object_flattened-schema.json
slug: factset-formula-cross_sectional_result_object_flattened
source_filename: factset-formula-cross_sectional_result_object_flattened-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"cross_sectional_result_object_flattened\",\n  \"type\": \"object\",\n  \"description\": \"\\nData model returned when the parameter **flatten=Y** is used in the request. This flattened, simplified JSON data returned from **flatten=Y** can be conceptualized as a table (rows and columns) where each data object in the result is a row in the table and the field names are the column names.\\n\\nThere will be one data object for each request containing the request, fsymId if requested, and Key-Value pairs for each data item (formula).\\n\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier requested.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"The **fsymId** field returned is the FactSet Default Permanent Identifier for the `requestId`. For all supported `requestId` symbol types, the `fsymId` parameter\
  \ will return the Regional Level PermId '-R' which identifies the securitys best regional security data series per currency. Currently, the fsymId parameter only supports equities. Accepted `requestId` symbol types include all FactSet Permanent Identifiers types, CUSIP, SEDOL, ISIN, and Tickers. Further documentation can be found at this [Online Assistant attachment](https://oa.apps.factset.com/cms/oaAttachment/64c3213a-f415-4c27-a336-92c73a72deed/24881). Included only if the `fsymId` parameter is set to Y.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-formula-cross_sectional_result_object_flattened-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: cross_sectional_result_object_flattened
---
