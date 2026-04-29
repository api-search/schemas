---
description: PayoutScheduleResponse schema from Adyen API
layout: schema
name: PayoutScheduleResponse
properties_list:
- description: The date of the next scheduled payout.
  name: nextScheduledPayout
  type: string
- description: 'The payout schedule of the account. Permitted values: `DEFAULT`, `DAILY`, `DAILY_US`, `DAILY_EU`, `DAILY_AU`, `DAILY_SG`, `WEEKLY`, `WEEKLY_ON_TUE_FRI_MIDNIGHT`, `BIWEEKLY_ON_1ST_AND_15TH_AT_MIDNIGHT`'
  name: schedule
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-payout-schedule-response-schema.json
slug: accounts-payout-schedule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-payout-schedule-response-schema.json\",\n  \"title\": \"PayoutScheduleResponse\",\n  \"description\": \"PayoutScheduleResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextScheduledPayout\": {\n      \"description\": \"The date of the next scheduled payout.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"description\": \"The payout schedule of the account.\\nPermitted values: `DEFAULT`, `DAILY`, `DAILY_US`, `DAILY_EU`, `DAILY_AU`, `DAILY_SG`, `WEEKLY`, `WEEKLY_ON_TUE_FRI_MIDNIGHT`, `BIWEEKLY_ON_1ST_AND_15TH_AT_MIDNIGHT`, `MONTHLY`, `HOLD`.\",\n      \"enum\": [\n        \"BIWEEKLY_ON_1ST_AND_15TH_AT_MIDNIGHT\",\n        \"DAILY\",\n        \"DAILY_AU\",\n        \"DAILY_EU\",\n        \"DAILY_SG\",\n        \"DAILY_US\"\
  ,\n        \"HOLD\",\n        \"MONTHLY\",\n        \"WEEKLY\",\n        \"WEEKLY_MON_TO_FRI_AU\",\n        \"WEEKLY_MON_TO_FRI_EU\",\n        \"WEEKLY_MON_TO_FRI_US\",\n        \"WEEKLY_ON_TUE_FRI_MIDNIGHT\",\n        \"WEEKLY_SUN_TO_THU_AU\",\n        \"WEEKLY_SUN_TO_THU_US\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-payout-schedule-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutScheduleResponse
---
