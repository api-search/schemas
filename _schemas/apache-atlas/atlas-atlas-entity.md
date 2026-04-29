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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entity-schema.json\",\n  \"title\": \"AtlasEntity\",\n  \"description\": \"Represents a single metadata entity in Apache Atlas.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"The type name of the entity.\",\n      \"example\": \"DataSet\"\n    },\n    \"guid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique identifier for the entity.\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Entity status (ACTIVE or DELETED).\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DELETED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Map of attribute name to attribute value.\",\n      \"example\": {\n        \"name\": \"customer_data\",\n        \"qualifiedName\": \"customer_data@prod\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Set of labels/tags applied to the entity.\",\n      \"example\": [\n        \"PII\",\n        \"Finance\"\n      ]\n    },\n    \"classifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Classifications applied to the entity.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-entity-schema.json
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
