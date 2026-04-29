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
source_filename: atlas-atlas-lineage-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-lineage-info-schema.json\",\n  \"title\": \"AtlasLineageInfo\",\n  \"description\": \"Lineage graph information for an entity showing upstream and downstream data flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseEntityGuid\": {\n      \"type\": \"string\",\n      \"description\": \"GUID of the entity whose lineage is being retrieved.\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"lineageDirection\": {\n      \"type\": \"string\",\n      \"description\": \"Direction of lineage traversal.\",\n      \"enum\": [\n        \"INPUT\",\n        \"OUTPUT\",\n        \"BOTH\"\n      ],\n      \"example\": \"BOTH\"\n    },\n    \"lineageDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of hops traversed in the lineage graph.\",\n  \
  \    \"example\": 3\n    },\n    \"guidEntityMap\": {\n      \"type\": \"object\",\n      \"description\": \"Map of GUID to entity header for all entities in the lineage graph.\"\n    },\n    \"relations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"List of lineage relationships between entities.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-lineage-info-schema.json
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
