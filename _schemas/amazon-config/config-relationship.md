---
description: The relationship of the related resource to the main resource.
layout: schema
name: Relationship
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
  name: relationshipName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-relationship-schema.json
slug: config-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-relationship-schema.json\",\n  \"title\": \"Relationship\",\n  \"description\": \"The relationship of the related resource to the main resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The resource type of the related resource.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the related resource (for example, <code>sg-xxxxxx</code>).\"\n        }\n      ]\n    },\n    \"resourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The custom name of the related resource, if available.\"\n        }\n      ]\n    },\n    \"relationshipName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipName\"\n        },\n        {\n          \"description\": \"The type of relationship with the related resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-relationship-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: Relationship
---
