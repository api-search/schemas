---
description: ListBonusPaymentsResponse schema from Amazon Mechanical Turk API
layout: schema
name: ListBonusPaymentsResponse
properties_list:
- description: ''
  name: NumResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: BonusPayments
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-list-bonus-payments-response-schema.json
slug: amazon-mechanical-turk-list-bonus-payments-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-bonus-payments-response-schema.json\",\n  \"title\": \"ListBonusPaymentsResponse\",\n  \"description\": \"ListBonusPaymentsResponse schema from Amazon Mechanical Turk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NumResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of bonus payments on this page in the filtered results list, equivalent to the number of bonus payments being returned by this call. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/PaginationToken\"\n    },\n    \"BonusPayments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BonusPaymentList\"\n        },\n\
  \        {\n          \"description\": \"A successful request to the ListBonusPayments operation returns a list of BonusPayment objects. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-list-bonus-payments-response-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: ListBonusPaymentsResponse
---
