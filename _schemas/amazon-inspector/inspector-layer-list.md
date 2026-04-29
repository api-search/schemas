---
description: LayerList schema
layout: schema
name: LayerList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-layer-list-schema.json
slug: inspector-layer-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-layer-list-schema.json\",\n  \"title\": \"LayerList\",\n  \"description\": \"LayerList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:[a-zA-Z0-9-]+:lambda:[a-zA-Z0-9-]+:\\\\d{12}:layer:[a-zA-Z0-9-_]+:[0-9]+$\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-layer-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: LayerList
---
