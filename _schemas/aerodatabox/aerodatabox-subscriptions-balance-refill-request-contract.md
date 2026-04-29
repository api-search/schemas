---
description: Represents a contract for refilling flight alert credits on a subscription.
layout: schema
name: SubscriptionsBalanceRefillRequestContract
properties_list:
- description: Number of credits to add to the notification subscription balance.
  name: credits
  type: integer
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-subscriptions-balance-refill-request-contract-schema.json
slug: aerodatabox-subscriptions-balance-refill-request-contract
source_filename: aerodatabox-subscriptions-balance-refill-request-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscriptions-balance-refill-request-contract-schema.json\",\n  \"title\": \"SubscriptionsBalanceRefillRequestContract\",\n  \"description\": \"Represents a contract for refilling flight alert credits on a subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"credits\": {\n      \"maximum\": 2147483647,\n      \"minimum\": 1,\n      \"type\": \"integer\",\n      \"description\": \"Number of credits to add to the notification subscription balance.\",\n      \"format\": \"int32\"\n    }\n  },\n  \"required\": [\n    \"credits\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscriptions-balance-refill-request-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SubscriptionsBalanceRefillRequestContract
---
