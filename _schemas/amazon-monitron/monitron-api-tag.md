---
description: A tag for a Monitron resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: key
  type: string
- description: Tag value.
  name: value
  type: string
provider_name: Amazon Monitron
provider_slug: amazon-monitron
schema_file: json-schema/monitron-api-tag-schema.json
slug: monitron-api-tag
source_filename: monitron-api-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A tag for a Monitron resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"Tag key.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Tag value.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-tag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Tag
---
