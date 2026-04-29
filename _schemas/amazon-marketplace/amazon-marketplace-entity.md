---
description: An entity contains data that describes your product, its supported features, and how it can be used or launched by your customer.
layout: schema
name: Entity
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: Identifier
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-entity-schema.json
slug: amazon-marketplace-entity
source_filename: amazon-marketplace-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-entity-schema.json\",\n  \"title\": \"Entity\",\n  \"description\": \"An entity contains data that describes your product, its supported features, and how it can be used or launched by your customer. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityType\"\n        },\n        {\n          \"description\": \"The type of entity.\"\n        }\n      ]\n    },\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The identifier for the entity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-entity-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: Entity
---
