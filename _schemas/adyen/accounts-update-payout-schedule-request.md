---
description: UpdatePayoutScheduleRequest schema from Adyen API
layout: schema
name: UpdatePayoutScheduleRequest
properties_list:
- description: 'Direction on how to handle any payouts that have already been scheduled. Permitted values: * `CLOSE` will close the existing batch of payouts. * `UPDATE` will reschedule the existing batch to the new '
  name: action
  type: string
- description: The reason for the payout schedule update. > This field is required when the `schedule` parameter is set to `HOLD`.
  name: reason
  type: string
- description: 'The payout schedule to which the account is to be updated. Permitted values: `DAILY`, `DAILY_US`, `DAILY_EU`, `DAILY_AU`, `DAILY_SG`, `WEEKLY`, `WEEKLY_ON_TUE_FRI_MIDNIGHT`, `BIWEEKLY_ON_1ST_AND_15TH_'
  name: schedule
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-update-payout-schedule-request-schema.json
slug: accounts-update-payout-schedule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-payout-schedule-request-schema.json\",\n  \"title\": \"UpdatePayoutScheduleRequest\",\n  \"description\": \"UpdatePayoutScheduleRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"Direction on how to handle any payouts that have already been scheduled.\\nPermitted values:\\n* `CLOSE` will close the existing batch of payouts.\\n* `UPDATE` will reschedule the existing batch to the new schedule.\\n* `NOTHING` (**default**) will allow the payout to proceed.\",\n      \"enum\": [\n        \"CLOSE\",\n        \"NOTHING\",\n        \"UPDATE\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"The reason for the payout schedule update.\\n> This field is required when the `schedule` parameter is\
  \ set to `HOLD`.\",\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"description\": \"The payout schedule to which the account is to be updated.\\nPermitted values: `DAILY`, `DAILY_US`, `DAILY_EU`, `DAILY_AU`, `DAILY_SG`, `WEEKLY`, `WEEKLY_ON_TUE_FRI_MIDNIGHT`, `BIWEEKLY_ON_1ST_AND_15TH_AT_MIDNIGHT`, `MONTHLY`, `HOLD`.\\n`HOLD` will prevent scheduled payouts from happening but will still allow manual payouts to occur.\",\n      \"enum\": [\n        \"BIWEEKLY_ON_1ST_AND_15TH_AT_MIDNIGHT\",\n        \"DAILY\",\n        \"DAILY_AU\",\n        \"DAILY_EU\",\n        \"DAILY_SG\",\n        \"DAILY_US\",\n        \"HOLD\",\n        \"MONTHLY\",\n        \"WEEKLY\",\n        \"WEEKLY_MON_TO_FRI_AU\",\n        \"WEEKLY_MON_TO_FRI_EU\",\n        \"WEEKLY_MON_TO_FRI_US\",\n        \"WEEKLY_ON_TUE_FRI_MIDNIGHT\",\n        \"WEEKLY_SUN_TO_THU_AU\",\n        \"WEEKLY_SUN_TO_THU_US\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"schedule\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-payout-schedule-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdatePayoutScheduleRequest
---
