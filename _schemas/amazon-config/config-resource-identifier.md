---
description: The details that identify a resource that is discovered by Config, including the resource type, ID, and (if available) the custom resource name.
layout: schema
name: ResourceIdentifier
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: resourceName
  type: object
- description: ''
  name: resourceDeletionTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-identifier-schema.json
slug: config-resource-identifier
source_filename: config-resource-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-identifier-schema.json\",\n  \"title\": \"ResourceIdentifier\",\n  \"description\": \"The details that identify a resource that is discovered by Config, including the resource type, ID, and (if available) the custom resource name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of resource.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the resource (for example, <code>sg-xxxxxx</code>).\"\n        }\n      ]\n    },\n    \"resourceName\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The custom name of the resource (if available).\"\n        }\n      ]\n    },\n    \"resourceDeletionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDeletionTime\"\n        },\n        {\n          \"description\": \"The time that the resource was deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-identifier-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceIdentifier
---
