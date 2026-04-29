---
description: Image and crop context for plant disease diagnosis.
layout: schema
name: Diagnose Request
properties_list:
- description: Crop identifier from the supported crops list.
  name: crop_id
  type: string
- description: Plant image file for diagnosis (JPEG or PNG).
  name: image
  type: string
provider_name: agrio
provider_slug: agrio
schema_file: json-schema/agrio-diagnose-request-schema.json
slug: agrio-diagnose-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnose-request-schema.json\",\n  \"title\": \"Diagnose Request\",\n  \"description\": \"Image and crop context for plant disease diagnosis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crop_id\": {\n      \"type\": \"string\",\n      \"description\": \"Crop identifier from the supported crops list.\",\n      \"example\": \"tomato\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Plant image file for diagnosis (JPEG or PNG).\"\n    }\n  },\n  \"required\": [\n    \"crop_id\",\n    \"image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agrio/refs/heads/main/json-schema/agrio-diagnose-request-schema.json
tags:
- Agriculture
- Plant Disease
- Pest Detection
- AI
- Crop Advisory
title: Diagnose Request
---
