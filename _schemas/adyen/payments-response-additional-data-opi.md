---
description: ResponseAdditionalDataOpi schema from Adyen API
layout: schema
name: ResponseAdditionalDataOpi
properties_list:
- description: 'Returned in the response if you included `opi.includeTransToken: true` in an ecommerce payment request. This contains an Oracle Payment Interface token that you can store in your Oracle Opera database'
  name: opi.transToken
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-response-additional-data-opi-schema.json
slug: payments-response-additional-data-opi
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-opi-schema.json\",\n  \"title\": \"ResponseAdditionalDataOpi\",\n  \"description\": \"ResponseAdditionalDataOpi schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"opi.transToken\": {\n      \"description\": \"Returned in the response if you included `opi.includeTransToken: true` in an ecommerce payment request. This contains an Oracle Payment Interface token that you can store in your Oracle Opera database to identify tokenized ecommerce transactions. For more information and required settings, see [Oracle Opera](https://docs.adyen.com/plugins/oracle-opera#opi-token-ecommerce).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-opi-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataOpi
---
