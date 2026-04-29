---
description: ''
layout: schema
name: SseConfigKeyArnString
properties_list: []
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-sse-config-key-arn-string-schema.json
slug: healthomics-sse-config-key-arn-string
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sse-config-key-arn-string-schema.json\",\n  \"title\": \"SseConfigKeyArnString\",\n  \"type\": \"string\",\n  \"pattern\": \".*arn:([^: ]*):([^: ]*):([^: ]*):([0-9]{12}):([^: ]*).*\",\n  \"minLength\": 20,\n  \"maxLength\": 2048\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sse-config-key-arn-string-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: SseConfigKeyArnString
---
