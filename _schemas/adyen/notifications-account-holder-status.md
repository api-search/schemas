---
description: AccountHolderStatus schema from Adyen API
layout: schema
name: AccountHolderStatus
properties_list:
- description: A list of events scheduled for the account holder.
  name: events
  type: array
- description: The payout state of the account holder.
  name: payoutState
  type: object
- description: The processing state of the account holder.
  name: processingState
  type: object
- description: 'The status of the account holder. >Permitted values: `Active`, `Inactive`, `Suspended`, `Closed`.'
  name: status
  type: string
- description: The reason why the status was assigned to the account holder.
  name: statusReason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-account-holder-status-schema.json
slug: notifications-account-holder-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-status-schema.json\",\n  \"title\": \"AccountHolderStatus\",\n  \"description\": \"AccountHolderStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"description\": \"A list of events scheduled for the account holder.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AccountEvent\"\n      },\n      \"type\": \"array\"\n    },\n    \"payoutState\": {\n      \"description\": \"The payout state of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountPayoutState\"\n    },\n    \"processingState\": {\n      \"description\": \"The processing state of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountProcessingState\"\n    },\n    \"status\": {\n      \"description\": \"The status of the\
  \ account holder.\\n>Permitted values: `Active`, `Inactive`, `Suspended`, `Closed`.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"Suspended\"\n      ],\n      \"type\": \"string\"\n    },\n    \"statusReason\": {\n      \"description\": \"The reason why the status was assigned to the account holder.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-account-holder-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountHolderStatus
---
