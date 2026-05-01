---
description: The configuration for bumpers. Bumpers are short audio or video clips that play at the start or before the end of an ad break. To learn more about bumpers, see <a href="https://docs.aws.amazon.com/mediatailor/latest/ug/bumpers.html">Bumpers</a>.
layout: schema
name: Bumper
properties_list:
- description: ''
  name: EndUrl
  type: object
- description: ''
  name: StartUrl
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-bumper-schema.json
slug: mediatailor-api-bumper
source_filename: mediatailor-api-bumper-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-bumper-schema.json\",\n  \"title\": \"Bumper\",\n  \"description\": \"The configuration for bumpers. Bumpers are short audio or video clips that play at the start or before the end of an ad break. To learn more about bumpers, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/bumpers.html\\\">Bumpers</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL for the end bumper asset.\"\n        }\n      ]\n    },\n    \"StartUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL for the start bumper asset.\"\n \
  \       }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-bumper-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Bumper
---
