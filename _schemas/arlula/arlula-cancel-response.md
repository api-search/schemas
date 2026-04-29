---
description: Response after cancelling a tasking campaign.
layout: schema
name: CancelResponse
properties_list:
- description: Whether the cancellation was successful.
  name: success
  type: boolean
- description: ID of the cancelled campaign.
  name: campaignId
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-cancel-response-schema.json
slug: arlula-cancel-response
source_filename: arlula-cancel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/cancel-response.json\",\n  \"title\": \"CancelResponse\",\n  \"description\": \"Response after cancelling a tasking campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cancellation was successful.\",\n      \"examples\": [\n        true\n      ]\n    },\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the cancelled campaign.\",\n      \"examples\": [\n        \"campaign-a1b2c3d4\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-cancel-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: CancelResponse
---
