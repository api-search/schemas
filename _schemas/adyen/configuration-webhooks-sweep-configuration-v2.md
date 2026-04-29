---
description: SweepConfigurationV2 schema from Adyen API
layout: schema
name: SweepConfigurationV2
properties_list:
- description: The destination or the source of the funds, depending on the sweep `type`. Either a `balanceAccountId`, `transferInstrumentId`, or `merchantAccount` is required.
  name: counterparty
  type: object
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes) in uppercase. For example, **EUR**. The sweep currency must match any of the [balances currencies](
  name: currency
  type: string
- description: The message that will be used in the sweep transfer's description body with a maximum length of 140 characters. If the message is longer after replacing placeholders, the message will be cut off at 14
  name: description
  type: string
- description: The unique identifier of the sweep.
  name: id
  type: string
- description: The reason for disabling the sweep.
  name: reason
  type: string
- description: The schedule when the `triggerAmount` is evaluated. If the balance meets the threshold, funds are pushed out of or pulled in to the balance account.
  name: schedule
  type: object
- description: 'The status of the sweep. If not provided, by default, this is set to **active**. Possible values: * **active**: the sweep is enabled and funds will be pulled in or pushed out based on the defined conf'
  name: status
  type: string
- description: The amount that must be pushed out or pulled in. You can configure either `sweepAmount` or `targetAmount`, not both.
  name: sweepAmount
  type: object
- description: The amount that must be available in the balance account after the sweep. You can configure either `sweepAmount` or `targetAmount`, not both.
  name: targetAmount
  type: object
- description: The threshold amount that triggers the sweep. If not provided, by default, the amount is set to zero. The `triggerAmount` is evaluated according to the specified `schedule.type`. * For `type` **pull**
  name: triggerAmount
  type: object
- description: 'The direction of sweep, whether pushing out or pulling in funds to the balance account. If not provided, by default, this is set to **push**. Possible values: * **push**: _push out funds_ to a destina'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-sweep-configuration-v2-schema.json
slug: configuration-webhooks-sweep-configuration-v2
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-sweep-configuration-v2-schema.json\",\n  \"title\": \"SweepConfigurationV2\",\n  \"description\": \"SweepConfigurationV2 schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"counterparty\": {\n      \"description\": \"The destination or the source of the funds, depending on the sweep `type`.\\n\\nEither a `balanceAccountId`, `transferInstrumentId`, or `merchantAccount` is required.\",\n      \"$ref\": \"#/components/schemas/SweepCounterparty\"\n    },\n    \"currency\": {\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes) in uppercase. For example, **EUR**.\\n\\nThe sweep currency must match any of the [balances currencies](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/get/balanceAccounts/{id}__resParam_balances).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The message that will be used in the sweep transfer's description body with a maximum length of 140 characters.\\n\\nIf the message is longer after replacing placeholders, the message will be cut off at 140 characters.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the sweep.\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"The reason for disabling the sweep.\",\n      \"enum\": [\n        \"amountLimitExceeded\",\n        \"approved\",\n        \"balanceAccountTemporarilyBlockedByTransactionRule\",\n        \"counterpartyAccountBlocked\",\n        \"counterpartyAccountClosed\",\n        \"counterpartyAccountNotFound\",\n        \"counterpartyAddressRequired\",\n        \"counterpartyBankTimedOut\",\n        \"counterpartyBankUnavailable\",\n        \"declinedByTransactionRule\",\n        \"error\",\n      \
  \  \"notEnoughBalance\",\n        \"refusedByCounterpartyBank\",\n        \"routeNotFound\",\n        \"scaFailed\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"description\": \"The schedule when the `triggerAmount` is evaluated. If the balance meets the threshold, funds are pushed out of or pulled in to the balance account.\",\n      \"$ref\": \"#/components/schemas/SweepSchedule\"\n    },\n    \"status\": {\n      \"description\": \"The status of the sweep. If not provided, by default, this is set to **active**.\\n\\nPossible values: \\n\\n * **active**:  the sweep is enabled and funds will be pulled in or pushed out based on the defined configuration. \\n\\n * **inactive**: the sweep is disabled and cannot be triggered. \\n\\n\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"type\": \"string\"\n    },\n    \"sweepAmount\": {\n      \"description\": \"The amount that must be pushed out or pulled in.\
  \ You can configure either `sweepAmount` or `targetAmount`, not both.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"targetAmount\": {\n      \"description\": \"The amount that must be available in the balance account after the sweep. You can configure either `sweepAmount` or `targetAmount`, not both.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"triggerAmount\": {\n      \"description\": \"The threshold amount that triggers the sweep. If not provided, by default, the amount is set to zero. The `triggerAmount` is evaluated according to the specified `schedule.type`.\\n\\n* For `type` **pull**, if the balance is less than or equal to the `triggerAmount`, funds are pulled in to the balance account.\\n\\n* For `type` **push**, if the balance is more than or equal to the `triggerAmount`, funds are pushed out of the balance account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"type\": {\n      \"default\": \"push\",\n      \"description\"\
  : \"The direction of sweep, whether pushing out or pulling in funds to the balance account. If not provided, by default, this is set to **push**.\\n\\nPossible values:\\n\\n * **push**: _push out funds_ to a destination balance account or transfer instrument.\\n\\n * **pull**: _pull in funds_ from a source merchant account, transfer instrument, or balance account.\",\n      \"enum\": [\n        \"pull\",\n        \"push\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"schedule\",\n    \"currency\",\n    \"counterparty\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-sweep-configuration-v2-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepConfigurationV2
---
