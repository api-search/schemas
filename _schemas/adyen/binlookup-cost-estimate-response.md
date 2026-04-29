---
description: CostEstimateResponse schema from Adyen API
layout: schema
name: CostEstimateResponse
properties_list:
- description: Card BIN details.
  name: cardBin
  type: object
- description: The estimated cost (scheme fee + interchange) in the settlement currency. If the settlement currency cannot be determined, the fee in EUR is returned.
  name: costEstimateAmount
  type: object
- description: Adyen's 16-character reference associated with the request.
  name: costEstimateReference
  type: string
- description: The result of the cost estimation.
  name: resultCode
  type: string
- description: 'Indicates the way the charges can be passed on to the cardholder. The following values are possible: * `ZERO` - the charges are not allowed to pass on * `PASSTHROUGH` - the charges can be passed on * '
  name: surchargeType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-cost-estimate-response-schema.json
slug: binlookup-cost-estimate-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-response-schema.json\",\n  \"title\": \"CostEstimateResponse\",\n  \"description\": \"CostEstimateResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardBin\": {\n      \"description\": \"Card BIN details.\",\n      \"$ref\": \"#/components/schemas/CardBin\"\n    },\n    \"costEstimateAmount\": {\n      \"description\": \"The estimated cost (scheme fee + interchange) in the settlement currency. If the settlement currency cannot be determined, the fee in EUR is returned.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"costEstimateReference\": {\n      \"x-addedInVersion\": \"52\",\n      \"description\": \"Adyen's 16-character reference associated with the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"\
  description\": \"The result of the cost estimation.\",\n      \"type\": \"string\"\n    },\n    \"surchargeType\": {\n      \"description\": \"Indicates the way the charges can be passed on to the cardholder. The following values are possible:\\n* `ZERO` - the charges are not allowed to pass on\\n* `PASSTHROUGH` - the charges can be passed on\\n* `UNLIMITED` - there is no limit on how much surcharge is passed on\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-cost-estimate-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CostEstimateResponse
---
