---
description: Error response
layout: schema
name: ErrorContract
properties_list:
- description: Error message
  name: message
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-error-contract-schema.json
slug: aerodatabox-error-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-error-contract-schema.json\",\n  \"title\": \"ErrorContract\",\n  \"description\": \"Error response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-error-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: ErrorContract
---
