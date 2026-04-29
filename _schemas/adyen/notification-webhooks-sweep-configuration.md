---
description: SweepConfiguration schema from Adyen API
layout: schema
name: SweepConfiguration
properties_list:
- description: The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id). You can only use this for periodic
  name: balanceAccountId
  type: string
- description: The unique identifier of the sweep.
  name: id
  type: string
- description: The merchant account that will be the source of funds. You can only use this if you are processing payments with Adyen. This can only be used for sweeps of `type` **pull** and `schedule.type` **balanc
  name: merchantAccount
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
- description: The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/transferInstruments__resParam_id). You can also use this in c
  name: transferInstrumentId
  type: string
- description: The threshold amount that triggers the sweep. If not provided, by default, the amount is set to zero. The `triggerAmount` is evaluated according to the specified `schedule.type`. * For `type` **pull**
  name: triggerAmount
  type: object
- description: 'The direction of sweep, whether pushing out or pulling in funds to the balance account. If not provided, by default, this is set to **push**. Possible values: * **push**: _push out funds_ to a destina'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-sweep-configuration-schema.json
slug: notification-webhooks-sweep-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-configuration-schema.json\",\n  \"title\": \"SweepConfiguration\",\n  \"description\": \"SweepConfiguration schema from Adyen API\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\\n\\n You can only use this for periodic sweep schedules such as `schedule.type` **daily** or **monthly**.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the sweep.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that will be the source of funds. You can only use this if you are processing payments\
  \ with Adyen. This can only be used for sweeps of `type` **pull** and `schedule.type` **balance**.\",\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"description\": \"The schedule when the `triggerAmount` is evaluated. If the balance meets the threshold, funds are pushed out of or pulled in to the balance account.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronSweepSchedule\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/SweepSchedule\"\n        }\n      ]\n    },\n    \"status\": {\n      \"x-enum\": [\n        {\n          \"description\": \"The sweep is enabled and funds will be pulled in or pushed out based on the defined configuration\",\n          \"value\": \"active\"\n        },\n        {\n          \"description\": \"The sweep is disabled and cannot be triggered.\",\n          \"value\": \"inactive\"\n        }\n      ],\n      \"description\": \"The status of the sweep. If not provided, by default, this\
  \ is set to **active**.\\n\\nPossible values: \\n\\n * **active**:  the sweep is enabled and funds will be pulled in or pushed out based on the defined configuration. \\n\\n * **inactive**: the sweep is disabled and cannot be triggered. \\n\\n\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"type\": \"string\"\n    },\n    \"sweepAmount\": {\n      \"description\": \"The amount that must be pushed out or pulled in. You can configure either `sweepAmount` or `targetAmount`, not both.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"targetAmount\": {\n      \"description\": \"The amount that must be available in the balance account after the sweep. You can configure either `sweepAmount` or `targetAmount`, not both.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/transferInstruments__resParam_id).\\\
  n\\nYou can also use this in combination with a `merchantAccount` and a `type` **pull** to start a direct debit request from the source transfer instrument. To use this feature, reach out to your Adyen contact.\",\n      \"type\": \"string\"\n    },\n    \"triggerAmount\": {\n      \"description\": \"The threshold amount that triggers the sweep. If not provided, by default, the amount is set to zero. The `triggerAmount` is evaluated according to the specified `schedule.type`.\\n\\n* For `type` **pull**, if the balance is less than or equal to the `triggerAmount`, funds are pulled in to the balance account.\\n\\n* For `type` **push**, if the balance is more than or equal to the `triggerAmount`, funds are pushed out of the balance account.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"type\": {\n      \"default\": \"push\",\n      \"description\": \"The direction of sweep, whether pushing out or pulling in funds to the balance account. If not provided, by default, this\
  \ is set to **push**.\\n\\nPossible values:\\n\\n * **push**: _push out funds_ to a destination balance account or transfer instrument.\\n\\n * **pull**: _pull in funds_ from a source merchant account, transfer instrument, or balance account.\",\n      \"enum\": [\n        \"pull\",\n        \"push\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"schedule\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepConfiguration
---
