---
description: Represents a single metadata entity in Apache Atlas.
layout: schema
name: AtlasEntity
properties_list:
- description: The type name of the entity.
  name: typeName
  type: string
- description: Globally unique identifier for the entity.
  name: guid
  type: string
- description: Entity status (ACTIVE or DELETED).
  name: status
  type: string
- description: Map of attribute name to attribute value.
  name: attributes
  type: object
- description: Set of labels/tags applied to the entity.
  name: labels
  type: array
- description: Classifications applied to the entity.
  name: classifications
  type: array
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-entity-schema.json
slug: atlas-atlas-entity
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasEntity
---
