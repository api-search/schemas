---
description: PayoutSettings schema from Adyen API
layout: schema
name: PayoutSettings
properties_list:
- description: 'Indicates if payouts to the bank account are allowed. This value is set automatically based on the status of the verification process. The value is: * **true** if `verificationStatus` is **valid**. * '
  name: allowed
  type: boolean
- description: 'Indicates if payouts to this bank account are enabled. Default: **true**. To receive payouts into this bank account, both `enabled` and `allowed` must be **true**.'
  name: enabled
  type: boolean
- description: 'The date when Adyen starts paying out to this bank account. Format: [ISO 8601](https://www.w3.org/TR/NOTE-datetime), for example, **2019-11-23T12:25:28Z** or **2020-05-27T20:25:28+08:00**. If not spec'
  name: enabledFromDate
  type: string
- description: The unique identifier of the payout setting.
  name: id
  type: string
- description: Determines how long it takes for the funds to reach the bank account. Adyen pays out based on the [payout frequency](https://docs.adyen.com/account/getting-paid#payout-frequency). Depending on the cur
  name: priority
  type: string
- description: The unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments) that contains the details of the bank account.
  name: transferInstrumentId
  type: string
- description: 'The status of the verification process for the bank account. Possible values: * **valid**: the verification was successful. * **pending**: the verification is in progress. * **invalid**: the informati'
  name: verificationStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payout-settings-schema.json
slug: management-payout-settings
source_filename: management-payout-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-schema.json\",\n  \"title\": \"PayoutSettings\",\n  \"description\": \"PayoutSettings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowed\": {\n      \"description\": \"Indicates if payouts to the bank account are allowed. This value is set automatically based on the status of the verification process. The value is:\\n\\n* **true** if `verificationStatus` is **valid**.\\n* **false** for all other values.\",\n      \"type\": \"boolean\"\n    },\n    \"enabled\": {\n      \"description\": \"Indicates if payouts to this bank account are enabled. Default: **true**.\\n\\nTo receive payouts into this bank account, both `enabled` and `allowed` must be **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"enabledFromDate\": {\n      \"description\": \"The date\
  \ when Adyen starts paying out to this bank account.\\n\\nFormat: [ISO 8601](https://www.w3.org/TR/NOTE-datetime), for example, **2019-11-23T12:25:28Z** or **2020-05-27T20:25:28+08:00**.\\n\\nIf not specified, the `enabled` field indicates if payouts are enabled for this bank account.\\n\\nIf a date is specified and:\\n\\n* `enabled`: **true**, payouts are enabled starting the specified date.\\n* `enabled`: **false**, payouts are disabled until the specified date. On the specified date, `enabled` changes to **true** and this field is reset to **null**.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the payout setting.\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"description\": \"Determines how long it takes for the funds to reach the bank account. Adyen pays out based on the [payout frequency](https://docs.adyen.com/account/getting-paid#payout-frequency). Depending on the currencies and banks involved in\
  \ transferring the money, it may take up to three days for the payout funds to arrive in the bank account.\\n\\n Possible values:\\n* **first**: same day.\\n* **urgent**: the next day.\\n* **normal**: between 1 and 3 days.\",\n      \"enum\": [\n        \"first\",\n        \"normal\",\n        \"urgent\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"The unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments) that contains the details of the bank account.\",\n      \"type\": \"string\"\n    },\n    \"verificationStatus\": {\n      \"description\": \"The status of the verification process for the bank account.\\n\\nPossible values:\\n* **valid**: the verification was successful.\\n* **pending**: the verification is in progress.\\n* **invalid**: the information provided is not complete.\\n* **rejected**:  there are reasons to refuse working with this entity.\"\
  ,\n      \"enum\": [\n        \"invalid\",\n        \"pending\",\n        \"rejected\",\n        \"valid\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"transferInstrumentId\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutSettings
---
