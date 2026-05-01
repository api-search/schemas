---
description: RemediationConfigurations schema
layout: schema
name: RemediationConfigurations
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-remediation-configurations-schema.json
slug: config-remediation-configurations
source_filename: config-remediation-configurations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-configurations-schema.json\",\n  \"title\": \"RemediationConfigurations\",\n  \"description\": \"RemediationConfigurations schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/RemediationConfiguration\"\n  },\n  \"minItems\": 0,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-configurations-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: RemediationConfigurations
---
