---
description: UpdateAccountHolderStateRequest schema from Adyen API
layout: schema
name: UpdateAccountHolderStateRequest
properties_list:
- description: The code of the Account Holder on which to update the state.
  name: accountHolderCode
  type: string
- description: If true, disable the requested state. If false, enable the requested state.
  name: disable
  type: boolean
- description: The reason that the state is being updated. >Required if the state is being disabled.
  name: reason
  type: string
- description: 'The state to be updated. >Permitted values are: `Processing`, `Payout`'
  name: stateType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-update-account-holder-state-request-schema.json
slug: accounts-update-account-holder-state-request
source_filename: accounts-update-account-holder-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-state-request-schema.json\",\n  \"title\": \"UpdateAccountHolderStateRequest\",\n  \"description\": \"UpdateAccountHolderStateRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder on which to update the state.\",\n      \"type\": \"string\"\n    },\n    \"disable\": {\n      \"description\": \"If true, disable the requested state.  If false, enable the requested state.\",\n      \"type\": \"boolean\"\n    },\n    \"reason\": {\n      \"description\": \"The reason that the state is being updated.\\n>Required if the state is being disabled.\",\n      \"type\": \"string\"\n    },\n    \"stateType\": {\n      \"description\": \"The state to be updated.\\n>Permitted values are:\
  \ `Processing`, `Payout`\",\n      \"enum\": [\n        \"LimitedPayout\",\n        \"LimitedProcessing\",\n        \"LimitlessPayout\",\n        \"LimitlessProcessing\",\n        \"Payout\",\n        \"Processing\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"stateType\",\n    \"disable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-state-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateAccountHolderStateRequest
---
