---
description: RecurringDetailsRequest schema from Adyen API
layout: schema
name: RecurringDetailsRequest
properties_list:
- description: The merchant account identifier you want to process the (transaction) request with.
  name: merchantAccount
  type: string
- description: A container for the type of a recurring contract to be retrieved. The contract value needs to match the contract value submitted in the payment transaction used to create a recurring contract. However
  name: recurring
  type: object
- description: The reference you use to uniquely identify the shopper (e.g. user ID or account ID).
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-recurring-details-request-schema.json
slug: recurring-recurring-details-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-details-request-schema.json\",\n  \"title\": \"RecurringDetailsRequest\",\n  \"description\": \"RecurringDetailsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier you want to process the (transaction) request with.\",\n      \"type\": \"string\"\n    },\n    \"recurring\": {\n      \"description\": \"A container for the type of a recurring contract to be retrieved.\\n\\nThe contract value needs to match the contract value submitted in the payment transaction used to create a recurring contract.\\nHowever, if `ONECLICK,RECURRING` is the original contract definition in the initial payment, then `contract` should take either `ONECLICK` or `RECURRING`, depending on whether or not you\
  \ want the shopper to enter their card's security code when they finalize their purchase.\",\n      \"$ref\": \"#/components/schemas/Recurring\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The reference you use to uniquely identify the shopper (e.g. user ID or account ID).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-details-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RecurringDetailsRequest
---
