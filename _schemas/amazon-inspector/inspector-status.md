---
description: Status schema
layout: schema
name: Status
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-status-schema.json
slug: inspector-status
source_filename: inspector-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-status-schema.json\",\n  \"title\": \"Status\",\n  \"description\": \"Status schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLING\",\n    \"ENABLED\",\n    \"DISABLING\",\n    \"DISABLED\",\n    \"SUSPENDING\",\n    \"SUSPENDED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-status-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Status
---
