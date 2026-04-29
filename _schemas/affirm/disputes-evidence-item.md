---
description: A single piece of evidence associated with a dispute.
layout: schema
name: EvidenceItem
properties_list:
- description: Unique identifier for this evidence item.
  name: id
  type: string
- description: Type of evidence (file, text, tracking).
  name: type
  type: string
- description: For text evidence, the content of the explanation. For file evidence, the file identifier.
  name: content
  type: string
- description: Timestamp when this evidence was submitted, in RFC 3339 format.
  name: submitted_at
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/disputes-evidence-item-schema.json
slug: disputes-evidence-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-evidence-item-schema.json\",\n  \"title\": \"EvidenceItem\",\n  \"description\": \"A single piece of evidence associated with a dispute.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this evidence item.\",\n      \"example\": \"500123\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of evidence (file, text, tracking).\",\n      \"enum\": [\n        \"file\",\n        \"text\",\n        \"tracking\"\n      ],\n      \"example\": \"file\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"For text evidence, the content of the explanation. For file evidence, the file identifier.\",\n      \"example\": \"example_value\"\n    },\n    \"submitted_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this evidence was submitted, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/disputes-evidence-item-schema.json
tags: []
title: EvidenceItem
---
