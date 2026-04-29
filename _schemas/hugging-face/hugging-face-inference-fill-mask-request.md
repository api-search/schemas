---
description: ''
layout: schema
name: FillMaskRequest
properties_list:
- description: Text with [MASK] token to fill
  name: inputs
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-fill-mask-request-schema.json
slug: hugging-face-inference-fill-mask-request
source_filename: hugging-face-inference-fill-mask-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FillMaskRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"string\",\n      \"description\": \"Text with [MASK] token to fill\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-fill-mask-request-schema.json
tags: []
title: FillMaskRequest
---
