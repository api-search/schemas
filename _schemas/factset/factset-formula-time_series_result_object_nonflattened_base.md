---
description: An object returning the results for a single identifier and formula. This is the base of the response object. The result attribute depends on the formula requested. Response objects with the various result attribute types are outlined in separate schemas.
layout: schema
name: time_series_result_object_nonflattened_base
properties_list:
- description: Indicates that there was an error in the execution of the FQL Formula. * Zero success * Non-zero failure
  name: error
  type: integer
- description: If error is non-zero, errorMessage will display the FQL formula error.
  name: errorMessage
  type: string
- description: FQL formula requested.
  name: formula
  type: string
- description: Display Name.
  name: displayName
  type: string
- description: Identifier requested.
  name: requestId
  type: string
- description: 'The **fsymId** field returned is the FactSet Default Permanent Identifier for the `requestId`. For all supported `requestId` symbol types, the `fsymId` parameter will return the Regional Level PermId '
  name: fsymId
  type: string
- description: Type of data returned in `result`
  name: dataType
  type: string
- description: Type of object returned in `result`
  name: objectType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-formula-time_series_result_object_nonflattened_base-schema.json
slug: factset-formula-time_series_result_object_nonflattened_base
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"time_series_result_object_nonflattened_base\",\n  \"type\": \"object\",\n  \"description\": \"An object returning the results for a single identifier and formula. This is the base of the response object. The result attribute depends on the formula requested. Response objects with the various result attribute types are outlined in separate schemas.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"integer\",\n      \"description\": \"Indicates that there was an error in the execution of the FQL Formula.\\n* Zero  success\\n* Non-zero  failure\\n\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"If error is non-zero, errorMessage will display the FQL formula error.\"\n    },\n    \"formula\": {\n      \"type\": \"string\",\n      \"description\": \"FQL formula requested.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Display Name.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier requested.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"The **fsymId** field returned is the FactSet Default Permanent Identifier for the `requestId`. For all supported `requestId` symbol types, the `fsymId` parameter will return the Regional Level PermId '-R' which identifies the securitys best regional security data series per currency. Currently, the fsymId parameter only supports equities. Accepted `requestId` symbol types include all FactSet Permanent Identifiers types, CUSIP, SEDOL, ISIN, and Tickers. Further documentation can be found at this [Online Assistant attachment](https://oa.apps.factset.com/cms/oaAttachment/64c3213a-f415-4c27-a336-92c73a72deed/24881). Included only if the `fsymId` parameter is set to Y.\\n\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data returned\
  \ in `result`\"\n    },\n    \"objectType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of object returned in `result`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-formula-time_series_result_object_nonflattened_base-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: time_series_result_object_nonflattened_base
---
