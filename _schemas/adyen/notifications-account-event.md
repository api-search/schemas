---
description: AccountEvent schema from Adyen API
layout: schema
name: AccountEvent
properties_list:
- description: 'The event. >Permitted values: `InactivateAccount`, `RefundNotPaidOutTransfers`. For more information, refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verificat'
  name: event
  type: string
- description: The date on which the event will take place.
  name: executionDate
  type: string
- description: The reason why this event has been created.
  name: reason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-event-schema.json
slug: notifications-account-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-event-schema.json\",\n  \"title\": \"AccountEvent\",\n  \"description\": \"AccountEvent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event\": {\n      \"description\": \"The event.\\n>Permitted values: `InactivateAccount`, `RefundNotPaidOutTransfers`.\\nFor more information, refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-process).\",\n      \"enum\": [\n        \"InactivateAccount\",\n        \"RefundNotPaidOutTransfers\"\n      ],\n      \"type\": \"string\"\n    },\n    \"executionDate\": {\n      \"description\": \"The date on which the event will take place.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"The reason why this event\
  \ has been created.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-event-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountEvent
---
