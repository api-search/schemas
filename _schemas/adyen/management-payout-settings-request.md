---
description: PayoutSettingsRequest schema from Adyen API
layout: schema
name: PayoutSettingsRequest
properties_list:
- description: 'Indicates if payouts to this bank account are enabled. Default: **true**. To receive payouts into this bank account, both `enabled` and `allowed` must be **true**.'
  name: enabled
  type: boolean
- description: 'The date when Adyen starts paying out to this bank account. Format: [ISO 8601](https://www.w3.org/TR/NOTE-datetime), for example, **2019-11-23T12:25:28Z** or **2020-05-27T20:25:28+08:00**. If not spec'
  name: enabledFromDate
  type: string
- description: The unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments) that contains the details of the bank account.
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payout-settings-request-schema.json
slug: management-payout-settings-request
source_filename: management-payout-settings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-request-schema.json\",\n  \"title\": \"PayoutSettingsRequest\",\n  \"description\": \"PayoutSettingsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"Indicates if payouts to this bank account are enabled. Default: **true**.\\n\\nTo receive payouts into this bank account, both `enabled` and `allowed` must be **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"enabledFromDate\": {\n      \"description\": \"The date when Adyen starts paying out to this bank account.\\n\\nFormat: [ISO 8601](https://www.w3.org/TR/NOTE-datetime), for example, **2019-11-23T12:25:28Z** or **2020-05-27T20:25:28+08:00**.\\n\\nIf not specified, the `enabled` field indicates if payouts are enabled for this bank account.\\n\\nIf a date\
  \ is specified and:\\n\\n* `enabled`: **true**, payouts are enabled starting the specified date.\\n* `enabled`: **false**, payouts are disabled until the specified date. On the specified date, `enabled` changes to **true** and this field is reset to **null**.\",\n      \"type\": \"string\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"The unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments) that contains the details of the bank account.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"transferInstrumentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutSettingsRequest
---
