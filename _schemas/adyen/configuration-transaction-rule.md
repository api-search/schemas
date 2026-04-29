---
description: TransactionRule schema from Adyen API
layout: schema
name: TransactionRule
properties_list:
- description: The level at which data must be accumulated, used in rules with `type` **velocity** or **maxUsage**. The level must be the [same or lower in hierarchy](https://docs.adyen.com/issuing/transaction-rules
  name: aggregationLevel
  type: string
- description: Your description for the transaction rule, maximum 300 characters.
  name: description
  type: string
- description: The date when the rule will stop being evaluated, in ISO 8601 extended offset date-time format. For example, **2020-12-18T10:15:30+01:00**. If not provided, the rule will be evaluated until the rule s
  name: endDate
  type: string
- description: The type and unique identifier of the resource to which the rule applies.
  name: entityKey
  type: object
- description: The unique identifier of the transaction rule.
  name: id
  type: string
- description: The [time interval](https://docs.adyen.com/issuing/transaction-rules#time-intervals) when the rule conditions apply.
  name: interval
  type: object
- description: The [outcome](https://docs.adyen.com/issuing/transaction-rules#outcome) that will be applied when a transaction meets the conditions of the rule. If not provided, by default, this is set to **hardBloc
  name: outcomeType
  type: string
- description: Your reference for the transaction rule, maximum 150 characters.
  name: reference
  type: string
- description: 'Indicates the type of request to which the rule applies. If not provided, by default, this is set to **authorization**. Possible values: **authorization**, **authentication**, **tokenization**, **bank'
  name: requestType
  type: string
- description: Contains one or more objects that define the [rule conditions](https://docs.adyen.com/issuing/transaction-rules#conditions). Each object must have a value and an operation which determines how the val
  name: ruleRestrictions
  type: object
- description: A positive or negative score applied to the transaction if it meets the conditions of the rule. Required when `outcomeType` is **scoreBased**. The value must be between **-100** and **100**.
  name: score
  type: integer
- description: The date when the rule will start to be evaluated, in ISO 8601 extended offset date-time format. For example, **2020-12-18T10:15:30+01:00**. If not provided when creating a transaction rule, the `star
  name: startDate
  type: string
- description: 'The status of the transaction rule. If you provide a `startDate` in the request, the rule is automatically created with an **active** status. Possible values: **active**, **inactive**.'
  name: status
  type: string
- description: 'The [type of rule](https://docs.adyen.com/issuing/transaction-rules#rule-types), which defines if a rule blocks transactions based on individual characteristics or accumulates data. Possible values: *'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rule-schema.json
slug: configuration-transaction-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-schema.json\",\n  \"title\": \"TransactionRule\",\n  \"description\": \"TransactionRule schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregationLevel\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The level at which data must be accumulated, used in rules with `type` **velocity** or **maxUsage**. The level must be the [same or lower in hierarchy](https://docs.adyen.com/issuing/transaction-rules#accumulate-data) than the `entityKey`.\\n\\nIf not provided, by default, the rule will accumulate data at the **paymentInstrument** level.\\n\\nPossible values: **paymentInstrument**, **paymentInstrumentGroup**, **balanceAccount**, **accountHolder**, **balancePlatform**.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n    \
  \  \"description\": \"Your description for the transaction rule, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"description\": \"The date when the rule will stop being evaluated, in ISO 8601 extended offset date-time format. For example, **2020-12-18T10:15:30+01:00**.\\n\\nIf not provided, the rule will be evaluated until the rule status is set to **inactive**.\",\n      \"type\": \"string\"\n    },\n    \"entityKey\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The type and unique identifier of the resource to which the rule applies.\",\n      \"$ref\": \"#/components/schemas/TransactionRuleEntityKey\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the transaction rule.\",\n      \"type\": \"string\"\n    },\n    \"interval\": {\n      \"description\": \"The [time interval](https://docs.adyen.com/issuing/transaction-rules#time-intervals) when the rule conditions apply.\"\
  ,\n      \"$ref\": \"#/components/schemas/TransactionRuleInterval\"\n    },\n    \"outcomeType\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The [outcome](https://docs.adyen.com/issuing/transaction-rules#outcome) that will be applied when a transaction meets the conditions of the rule. If not provided, by default, this is set to **hardBlock**.\\n\\nPossible values:\\n\\n * **hardBlock**: the transaction is declined.\\n\\n* **scoreBased**: the transaction is assigned the `score` you specified. Adyen calculates the total score and if it exceeds 100, the transaction is declined.\",\n      \"enum\": [\n        \"enforceSCA\",\n        \"hardBlock\",\n        \"scoreBased\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the transaction rule, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"requestType\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\"\
  : \"Indicates the type of request to which the rule applies. If not provided, by default, this is set to **authorization**.\\n\\nPossible values: **authorization**, **authentication**, **tokenization**, **bankTransfer**.\",\n      \"enum\": [\n        \"authentication\",\n        \"authorization\",\n        \"bankTransfer\",\n        \"tokenization\"\n      ],\n      \"type\": \"string\"\n    },\n    \"ruleRestrictions\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Contains one or more objects that define the [rule conditions](https://docs.adyen.com/issuing/transaction-rules#conditions). Each object must have a value and an operation which determines how the values must be evaluated.\\n\\nFor example, a `countries` object can have a list of country codes **[\\\"US\\\", \\\"CA\\\"]** in the `value` field and **anyMatch** in the `operation` field.\",\n      \"$ref\": \"#/components/schemas/TransactionRuleRestrictions\"\n    },\n    \"score\": {\n      \"x-addedInVersion\"\
  : \"2\",\n      \"description\": \"A positive or negative score applied to the transaction if it meets the conditions of the rule. Required when `outcomeType` is **scoreBased**.  The value must be between **-100** and **100**.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"startDate\": {\n      \"description\": \"The date when the rule will start to be evaluated, in ISO 8601 extended offset date-time format. For example, **2020-12-18T10:15:30+01:00**.\\n\\nIf not provided when creating a transaction rule, the `startDate` is set to the date when the rule status is set to **active**. \\n\\n\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the transaction rule. If you provide a `startDate` in the request, the rule is automatically created \\nwith an **active** status. \\n\\nPossible values: **active**, **inactive**.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"type\": \"string\"\
  \n    },\n    \"type\": {\n      \"description\": \"The [type of rule](https://docs.adyen.com/issuing/transaction-rules#rule-types), which defines if a rule blocks transactions based on individual characteristics or accumulates data.\\n\\nPossible values:\\n * **blockList**: decline a transaction when the conditions are met.\\n * **maxUsage**: add the amount or number of transactions for the lifetime of a payment instrument, and then decline a transaction when the specified limits are met.\\n * **velocity**: add the amount or number of transactions based on a specified time interval, and then decline a transaction when the specified limits are met.\\n\",\n      \"enum\": [\n        \"allowList\",\n        \"blockList\",\n        \"maxUsage\",\n        \"velocity\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"description\",\n    \"reference\",\n    \"entityKey\",\n    \"interval\",\n    \"ruleRestrictions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRule
---
