---
description: Multiple entities with extended information for bulk operations.
layout: schema
name: AtlasEntitiesWithExtInfo
properties_list:
- description: List of entities to create or update.
  name: entities
  type: array
- description: Map of referenced entities.
  name: referredEntities
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-entities-with-ext-info-schema.json
slug: atlas-atlas-entities-with-ext-info
source_filename: atlas-atlas-entities-with-ext-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entities-with-ext-info-schema.json\",\n  \"title\": \"AtlasEntitiesWithExtInfo\",\n  \"description\": \"Multiple entities with extended information for bulk operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AtlasEntity\"\n      },\n      \"description\": \"List of entities to create or update.\"\n    },\n    \"referredEntities\": {\n      \"type\": \"object\",\n      \"description\": \"Map of referenced entities.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entities-with-ext-info-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasEntitiesWithExtInfo
---
