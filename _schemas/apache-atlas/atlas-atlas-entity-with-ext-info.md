---
description: Entity with extended information for create/update operations.
layout: schema
name: AtlasEntityWithExtInfo
properties_list:
- description: ''
  name: entity
  type: object
- description: Map of referenced entities.
  name: referredEntities
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-entity-with-ext-info-schema.json
slug: atlas-atlas-entity-with-ext-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entity-with-ext-info-schema.json\",\n  \"title\": \"AtlasEntityWithExtInfo\",\n  \"description\": \"Entity with extended information for create/update operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity\": {\n      \"$ref\": \"#/components/schemas/AtlasEntity\"\n    },\n    \"referredEntities\": {\n      \"type\": \"object\",\n      \"description\": \"Map of referenced entities.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entity-with-ext-info-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasEntityWithExtInfo
---
