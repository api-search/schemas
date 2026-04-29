---
description: Specifies whether the configuration recorder excludes resource types from being recorded. Use the <code>resourceTypes</code> field to enter a comma-separated list of resource types to exclude as exemptions.
layout: schema
name: ExclusionByResourceTypes
properties_list:
- description: ''
  name: resourceTypes
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-exclusion-by-resource-types-schema.json
slug: config-exclusion-by-resource-types
source_filename: config-exclusion-by-resource-types-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-exclusion-by-resource-types-schema.json\",\n  \"title\": \"ExclusionByResourceTypes\",\n  \"description\": \"Specifies whether the configuration recorder excludes resource types from being recorded. Use the <code>resourceTypes</code> field to enter a comma-separated list of resource types to exclude as exemptions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypeList\"\n        },\n        {\n          \"description\": \"A comma-separated list of resource types to exclude from recording by the configuration recorder.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-exclusion-by-resource-types-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ExclusionByResourceTypes
---
