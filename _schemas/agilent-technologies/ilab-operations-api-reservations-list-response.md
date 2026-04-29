---
description: List of reservations for a core facility.
layout: schema
name: Reservations List Response
properties_list:
- description: ''
  name: reservations
  type: array
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-reservations-list-response-schema.json
slug: ilab-operations-api-reservations-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-reservations-list-response-schema.json\",\n  \"title\": \"Reservations List Response\",\n  \"description\": \"List of reservations for a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reservations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Reservation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-reservations-list-response-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Reservations List Response
---
