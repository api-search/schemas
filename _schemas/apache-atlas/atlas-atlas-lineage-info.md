---
description: Lineage graph information for an entity showing upstream and downstream data flow.
layout: schema
name: AtlasLineageInfo
properties_list:
- description: GUID of the entity whose lineage is being retrieved.
  name: baseEntityGuid
  type: string
- description: Direction of lineage traversal.
  name: lineageDirection
  type: string
- description: Number of hops traversed in the lineage graph.
  name: lineageDepth
  type: integer
- description: Map of GUID to entity header for all entities in the lineage graph.
  name: guidEntityMap
  type: object
- description: List of lineage relationships between entities.
  name: relations
  type: array
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-lineage-info-schema.json
slug: atlas-atlas-lineage-info
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasLineageInfo
---
