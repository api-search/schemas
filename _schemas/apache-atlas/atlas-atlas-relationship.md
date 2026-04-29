---
description: A relationship between two Atlas entities.
layout: schema
name: AtlasRelationship
properties_list:
- description: GUID of the relationship.
  name: guid
  type: string
- description: Type name of the relationship.
  name: typeName
  type: string
- description: Status of the relationship.
  name: status
  type: string
- description: First endpoint of the relationship.
  name: end1
  type: object
- description: Second endpoint of the relationship.
  name: end2
  type: object
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-relationship-schema.json
slug: atlas-atlas-relationship
source_filename: atlas-atlas-relationship-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-relationship-schema.json\",\n  \"title\": \"AtlasRelationship\",\n  \"description\": \"A relationship between two Atlas entities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"guid\": {\n      \"type\": \"string\",\n      \"description\": \"GUID of the relationship.\",\n      \"example\": \"rel-guid-001\"\n    },\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"Type name of the relationship.\",\n      \"example\": \"DataSetLineage\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the relationship.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DELETED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"end1\": {\n      \"type\": \"object\",\n      \"description\": \"First endpoint of the relationship.\"\
  ,\n      \"properties\": {\n        \"guid\": {\n          \"type\": \"string\",\n          \"example\": \"source-entity-guid\"\n        },\n        \"typeName\": {\n          \"type\": \"string\",\n          \"example\": \"DataSet\"\n        }\n      }\n    },\n    \"end2\": {\n      \"type\": \"object\",\n      \"description\": \"Second endpoint of the relationship.\",\n      \"properties\": {\n        \"guid\": {\n          \"type\": \"string\",\n          \"example\": \"target-entity-guid\"\n        },\n        \"typeName\": {\n          \"type\": \"string\",\n          \"example\": \"DataSet\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-relationship-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasRelationship
---
