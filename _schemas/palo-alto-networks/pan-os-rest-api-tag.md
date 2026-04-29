---
description: A tag for categorizing configuration objects.
layout: schema
name: Tag
properties_list:
- description: Unique name of the tag.
  name: '@name'
  type: string
- description: Display color for the tag (e.g., color1, color2).
  name: color
  type: string
- description: Description or comments for the tag.
  name: comments
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-tag-schema.json
slug: pan-os-rest-api-tag
source_filename: pan-os-rest-api-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"description\": \"A tag for categorizing configuration objects.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-tag-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the tag.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Display color for the tag (e.g., color1, color2).\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Description or comments for the tag.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-tag-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Tag
---
