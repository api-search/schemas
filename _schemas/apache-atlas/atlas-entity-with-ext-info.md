---
description: An entity with its extended information (referred entities, classifications).
layout: schema
name: EntityWithExtInfo
properties_list:
- description: ''
  name: entity
  type: object
- description: Map of GUID to related entity for entities referenced by this entity.
  name: referredEntities
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-entity-with-ext-info-schema.json
slug: atlas-entity-with-ext-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-entity-with-ext-info-schema.json\",\n  \"title\": \"EntityWithExtInfo\",\n  \"description\": \"An entity with its extended information (referred entities, classifications).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entity\": {\n      \"$ref\": \"#/components/schemas/AtlasEntity\"\n    },\n    \"referredEntities\": {\n      \"type\": \"object\",\n      \"description\": \"Map of GUID to related entity for entities referenced by this entity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-entity-with-ext-info-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: EntityWithExtInfo
---
