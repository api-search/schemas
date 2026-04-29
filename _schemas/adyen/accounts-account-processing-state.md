---
description: AccountProcessingState schema from Adyen API
layout: schema
name: AccountProcessingState
properties_list:
- description: The reason why processing has been disabled.
  name: disableReason
  type: string
- description: Indicates whether the processing of payments is allowed.
  name: disabled
  type: boolean
- description: The lower bound of the processing tier (i.e., an account holder must have processed at least this amount of money in order to be placed into this tier).
  name: processedFrom
  type: object
- description: The upper bound of the processing tier (i.e., an account holder must have processed less than this amount of money in order to be placed into this tier).
  name: processedTo
  type: object
- description: The processing tier that the account holder occupies.
  name: tierNumber
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-account-processing-state-schema.json
slug: accounts-account-processing-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-account-processing-state-schema.json\",\n  \"title\": \"AccountProcessingState\",\n  \"description\": \"AccountProcessingState schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disableReason\": {\n      \"description\": \"The reason why processing has been disabled.\",\n      \"type\": \"string\"\n    },\n    \"disabled\": {\n      \"description\": \"Indicates whether the processing of payments is allowed.\",\n      \"type\": \"boolean\"\n    },\n    \"processedFrom\": {\n      \"description\": \"The lower bound of the processing tier (i.e., an account holder must have processed at least this amount of money in order to be placed into this tier).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"processedTo\": {\n      \"description\": \"The upper bound of the\
  \ processing tier (i.e., an account holder must have processed less than this amount of money in order to be placed into this tier).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"tierNumber\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The processing tier that the account holder occupies.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-account-processing-state-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountProcessingState
---
