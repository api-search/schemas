---
description: A format-specific representation or rendition of a library element.
layout: schema
name: Representation
properties_list:
- description: Unique identifier of the representation.
  name: id
  type: string
- description: Format type of the representation.
  name: type
  type: string
- description: Representation content payload (format depends on element type).
  name: content
  type: object
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-representation-schema.json
slug: creative-cloud-libraries-representation
source_filename: creative-cloud-libraries-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-representation-schema.json\",\n  \"title\": \"Representation\",\n  \"description\": \"A format-specific representation or rendition of a library element.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the representation.\",\n      \"example\": \"rep-001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Format type of the representation.\",\n      \"example\": \"application/vnd.adobe.element.color+dcx\"\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"Representation content payload (format depends on element type).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-representation-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: Representation
---
