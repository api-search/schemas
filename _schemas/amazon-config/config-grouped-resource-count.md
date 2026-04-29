---
description: The count of resources that are grouped by the group name.
layout: schema
name: GroupedResourceCount
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: ResourceCount
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-grouped-resource-count-schema.json
slug: config-grouped-resource-count
source_filename: config-grouped-resource-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-grouped-resource-count-schema.json\",\n  \"title\": \"GroupedResourceCount\",\n  \"description\": \"The count of resources that are grouped by the group name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The name of the group that can be region, account ID, or resource type. For example, region1, region2 if the region was chosen as <code>GroupByKey</code>.\"\n        }\n      ]\n    },\n    \"ResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of resources in the group.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"GroupName\",\n    \"ResourceCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-grouped-resource-count-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GroupedResourceCount
---
