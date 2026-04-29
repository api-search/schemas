---
description: Filters the results by resource account ID, region, resource ID, and resource name.
layout: schema
name: ResourceFilters
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ResourceName
  type: object
- description: ''
  name: Region
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-filters-schema.json
slug: config-resource-filters
source_filename: config-resource-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-filters-schema.json\",\n  \"title\": \"ResourceFilters\",\n  \"description\": \"Filters the results by resource account ID, region, resource ID, and resource name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit source account ID.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the resource.\"\n        }\n      ]\n    },\n    \"ResourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n    \
  \      \"description\": \"The name of the resource.\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-filters-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceFilters
---
