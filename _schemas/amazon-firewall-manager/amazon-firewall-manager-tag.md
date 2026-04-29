---
description: A key-value metadata label applied to a Firewall Manager resource.
layout: schema
name: Tag
properties_list:
- description: Tag key.
  name: Key
  type: string
- description: Tag value.
  name: Value
  type: string
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
schema_file: json-schema/amazon-firewall-manager-tag-schema.json
slug: amazon-firewall-manager-tag
source_filename: amazon-firewall-manager-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key-value metadata label applied to a Firewall Manager resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"Tag key.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"Tag value.\"\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-tag-schema.json
tags:
- AWS
- Compliance
- Firewall
- Network Security
- Security
title: Tag
---
