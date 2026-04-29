---
description: UpdatePayoutSettingsRequest schema from Adyen API
layout: schema
name: UpdatePayoutSettingsRequest
properties_list:
- description: 'Indicates if payouts to this bank account are enabled. Default: **true**. To receive payouts into this bank account, both `enabled` and `allowed` must be **true**.'
  name: enabled
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-payout-settings-request-schema.json
slug: management-update-payout-settings-request
source_filename: management-update-payout-settings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-payout-settings-request-schema.json\",\n  \"title\": \"UpdatePayoutSettingsRequest\",\n  \"description\": \"UpdatePayoutSettingsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"Indicates if payouts to this bank account are enabled. Default: **true**.\\n\\nTo receive payouts into this bank account, both `enabled` and `allowed` must be **true**.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-payout-settings-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdatePayoutSettingsRequest
---
