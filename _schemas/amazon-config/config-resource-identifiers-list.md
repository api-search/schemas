---
description: ResourceIdentifiersList schema
layout: schema
name: ResourceIdentifiersList
properties_list: []
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-identifiers-list-schema.json
slug: config-resource-identifiers-list
source_filename: config-resource-identifiers-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-identifiers-list-schema.json\",\n  \"title\": \"ResourceIdentifiersList\",\n  \"description\": \"ResourceIdentifiersList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AggregateResourceIdentifier\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-identifiers-list-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceIdentifiersList
---
