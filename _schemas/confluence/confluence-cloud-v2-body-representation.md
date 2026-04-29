---
description: ''
layout: schema
name: BodyRepresentation
properties_list:
- description: The name of the representation format.
  name: representation
  type: string
- description: The body content in this representation.
  name: value
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-body-representation-schema.json
slug: confluence-cloud-v2-body-representation
source_filename: confluence-cloud-v2-body-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BodyRepresentation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"representation\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the representation format.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The body content in this representation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-body-representation-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: BodyRepresentation
---
