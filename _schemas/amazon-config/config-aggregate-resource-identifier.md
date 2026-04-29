---
description: The details that identify a resource that is collected by Config aggregator, including the resource type, ID, (if available) the custom resource name, the source account, and source region.
layout: schema
name: AggregateResourceIdentifier
properties_list:
- description: ''
  name: SourceAccountId
  type: object
- description: ''
  name: SourceRegion
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-resource-identifier-schema.json
slug: config-aggregate-resource-identifier
source_filename: config-aggregate-resource-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-resource-identifier-schema.json\",\n  \"title\": \"AggregateResourceIdentifier\",\n  \"description\": \"The details that identify a resource that is collected by Config aggregator, including the resource type, ID, (if available) the custom resource name, the source account, and source region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the source account.\"\n        }\n      ]\n    },\n    \"SourceRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region where data is aggregated.\"\
  \n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"ResourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the Amazon Web Services resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceAccountId\",\n    \"SourceRegion\",\n    \"ResourceId\",\n    \"ResourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-resource-identifier-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateResourceIdentifier
---
