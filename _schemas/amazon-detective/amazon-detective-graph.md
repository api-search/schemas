---
description: A behavior graph in Amazon Detective
layout: schema
name: Graph
properties_list:
- description: The ARN of the behavior graph.
  name: Arn
  type: string
- description: The date and time that the behavior graph was created.
  name: CreatedTime
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-graph-schema.json
slug: amazon-detective-graph
source_filename: amazon-detective-graph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-graph-schema.json\",\n  \"title\": \"Graph\",\n  \"description\": \"A behavior graph in Amazon Detective\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the behavior graph was created.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-graph-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: Graph
---
