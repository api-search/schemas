---
description: Describes subscriber (consumer of the subscription)
layout: schema
name: SubscriberContract
properties_list:
- description: Type of subscriber. Completemented by SubscriberId.
  name: type
  type: string
- description: ID
  name: id
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-subscriber-contract-schema.json
slug: aerodatabox-subscriber-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscriber-contract-schema.json\",\n  \"title\": \"SubscriberContract\",\n  \"description\": \"Describes subscriber (consumer of the subscription)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Type of subscriber. Completemented by SubscriberId.\"\n    },\n    \"id\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"ID\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscriber-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SubscriberContract
---
