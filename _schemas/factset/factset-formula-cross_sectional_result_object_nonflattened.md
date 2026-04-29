---
description: An object returning the results for a single formula.
layout: schema
name: cross_sectional_result_object_nonflattened
properties_list:
- description: If `universe` is submitted instead of `ids`, then the universe attribute will display the universe expression requested.
  name: universe
  type: string
- description: Name of data item (requestId, requested Screening formula, or fsymId)
  name: dataItemName
  type: string
- description: Display Name.
  name: displayName
  type: string
- description: ''
  name: result
  type: array
- description: Data type of the data item
  name: dataType
  type: string
- description: Data item error indicator. * Zero success * Non-zero failure
  name: error
  type: integer
- description: If error is non-zero, errorMessage will display the Screening formula error.
  name: errorMessage
  type: string
- description: Screening formula warnings. This attribute is only displayed if warnings are generated in the execution of the Screening formula.
  name: warnings
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-formula-cross_sectional_result_object_nonflattened-schema.json
slug: factset-formula-cross_sectional_result_object_nonflattened
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"cross_sectional_result_object_nonflattened\",\n  \"type\": \"object\",\n  \"description\": \"An object returning the results for a single formula.\",\n  \"properties\": {\n    \"universe\": {\n      \"type\": \"string\",\n      \"description\": \"If `universe` is submitted instead of `ids`, then the universe attribute will display the universe expression requested.\"\n    },\n    \"dataItemName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of data item (requestId, requested Screening formula, or fsymId)\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display Name.\"\n    },\n    \"result\": {\n      \"type\": \"array\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the data item\"\n    },\n    \"error\": {\n      \"type\": \"integer\",\n      \"description\": \"Data item error indicator.\\\
  n * Zero  success\\n * Non-zero  failure\\n\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"If error is non-zero, errorMessage will display the Screening formula error.\"\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"Screening formula warnings. This attribute is only displayed if warnings are generated in the execution of the Screening formula.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-formula-cross_sectional_result_object_nonflattened-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: cross_sectional_result_object_nonflattened
---
