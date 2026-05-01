---
description: This object is a container for common summary information about the entity. The summary doesn't contain the whole entity structure, but it does contain information common across all entities.
layout: schema
name: EntitySummary
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: EntityType
  type: object
- description: ''
  name: EntityId
  type: object
- description: ''
  name: EntityArn
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Visibility
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-entity-summary-schema.json
slug: amazon-marketplace-entity-summary
source_filename: amazon-marketplace-entity-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-entity-summary-schema.json\",\n  \"title\": \"EntitySummary\",\n  \"description\": \"This object is a container for common summary information about the entity. The summary doesn't contain the whole entity structure, but it does contain information common across all entities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityNameString\"\n        },\n        {\n          \"description\": \"The name for the entity. This value is not unique. It is defined by the seller.\"\n        }\n      ]\n    },\n    \"EntityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityType\"\n        },\n        {\n          \"description\": \"The type of the entity.\"\n\
  \        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the entity.\"\n        }\n      ]\n    },\n    \"EntityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated with the unique identifier for the entity.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The last time the entity was published, using ISO 8601 format (2018-02-27T13:45:22Z).\"\n        }\n      ]\n    },\n    \"Visibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VisibilityValue\"\n        },\n        {\n          \"description\": \"The visibility status of the entity\
  \ to buyers. This value can be <code>Public</code> (everyone can view the entity), <code>Limited</code> (the entity is visible to limited accounts only), or <code>Restricted</code> (the entity was published and then unpublished and only existing buyers can view it). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-entity-summary-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: EntitySummary
---
