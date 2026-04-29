---
description: Runtime schema
layout: schema
name: Runtime
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-runtime-schema.json
slug: inspector-runtime
source_filename: inspector-runtime-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-runtime-schema.json\",\n  \"title\": \"Runtime\",\n  \"description\": \"Runtime schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NODEJS\",\n    \"NODEJS_12_X\",\n    \"NODEJS_14_X\",\n    \"NODEJS_16_X\",\n    \"JAVA_8\",\n    \"JAVA_8_AL2\",\n    \"JAVA_11\",\n    \"PYTHON_3_7\",\n    \"PYTHON_3_8\",\n    \"PYTHON_3_9\",\n    \"UNSUPPORTED\",\n    \"NODEJS_18_X\",\n    \"GO_1_X\",\n    \"JAVA_17\",\n    \"PYTHON_3_10\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-runtime-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Runtime
---
