---
description: Collection of all type definitions in Apache Atlas.
layout: schema
name: AtlasTypesDef
properties_list:
- description: Entity type definitions.
  name: entityDefs
  type: array
- description: Classification type definitions.
  name: classificationDefs
  type: array
- description: Enumeration type definitions.
  name: enumDefs
  type: array
- description: Relationship type definitions.
  name: relationshipDefs
  type: array
- description: Business metadata type definitions.
  name: businessMetadataDefs
  type: array
provider_name: Apache Atlas
provider_slug: apache-atlas
schema_file: json-schema/atlas-atlas-types-def-schema.json
slug: atlas-atlas-types-def
source_filename: atlas-atlas-types-def-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-types-def-schema.json\",\n  \"title\": \"AtlasTypesDef\",\n  \"description\": \"Collection of all type definitions in Apache Atlas.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityDefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Entity type definitions.\"\n    },\n    \"classificationDefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Classification type definitions.\"\n    },\n    \"enumDefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Enumeration type definitions.\"\n    },\n    \"relationshipDefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"object\"\n      },\n      \"description\": \"Relationship type definitions.\"\n    },\n    \"businessMetadataDefs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Business metadata type definitions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-atlas/refs/heads/main/json-schema/atlas-atlas-types-def-schema.json
tags:
- Apache
- Big Data
- Compliance
- Data Governance
- Data Lineage
- Hadoop
- Metadata
- Open Source
title: AtlasTypesDef
---
