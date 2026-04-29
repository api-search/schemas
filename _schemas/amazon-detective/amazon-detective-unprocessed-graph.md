---
description: A behavior graph that could not be processed
layout: schema
name: UnprocessedGraph
properties_list:
- description: The ARN of the organization behavior graph.
  name: GraphArn
  type: string
- description: The reason data source package information could not be retrieved for the behavior graph.
  name: Reason
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-unprocessed-graph-schema.json
slug: amazon-detective-unprocessed-graph
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-unprocessed-graph-schema.json\",\n  \"title\": \"UnprocessedGraph\",\n  \"description\": \"A behavior graph that could not be processed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organization behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason data source package information could not be retrieved for the behavior graph.\",\n      \"example\": \"Graph not found\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-unprocessed-graph-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: UnprocessedGraph
---
