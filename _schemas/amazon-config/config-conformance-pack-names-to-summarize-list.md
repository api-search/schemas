---
description: ConformancePackNamesToSummarizeList schema
layout: schema
name: ConformancePackNamesToSummarizeList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-names-to-summarize-list-schema.json
slug: config-conformance-pack-names-to-summarize-list
source_filename: config-conformance-pack-names-to-summarize-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-names-to-summarize-list-schema.json\",\n  \"title\": \"ConformancePackNamesToSummarizeList\",\n  \"description\": \"ConformancePackNamesToSummarizeList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ConformancePackName\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 5\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-names-to-summarize-list-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackNamesToSummarizeList
---
