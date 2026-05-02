---
description: Represents a data entity in the Microsoft Purview Data Map, based on the Apache Atlas entity model. Entities are the core building blocks of the data catalog.
layout: schema
name: Microsoft Purview Atlas Entity
properties_list:
- description: The attributes of the entity, defined by its type definition
  name: attributes
  type: object
- description: The name of the entity type (e.g., azure_sql_table, azure_blob_path)
  name: typeName
  type: string
- description: ETag for concurrency control
  name: lastModifiedTS
  type: string
- description: Business metadata attributes attached to the entity
  name: businessAttributes
  type: object
- description: Classifications applied to the entity
  name: classifications
  type: array
- description: The creation time of the entity in epoch milliseconds
  name: createTime
  type: integer
- description: The user who created the entity
  name: createdBy
  type: string
- description: The globally unique identifier of the entity
  name: guid
  type: string
- description: The home identifier
  name: homeId
  type: string
- description: Labels applied to the entity
  name: labels
  type: array
- description: Glossary term assignments for the entity
  name: meanings
  type: array
- description: The provenance type of the entity
  name: provenanceType
  type: integer
- description: Whether the entity is a proxy
  name: proxy
  type: boolean
- description: Relationship attributes of the entity
  name: relationshipAttributes
  type: object
- description: The status of the entity
  name: status
  type: string
- description: The last update time of the entity in epoch milliseconds
  name: updateTime
  type: integer
- description: The user who last updated the entity
  name: updatedBy
  type: string
- description: The version number of the entity
  name: version
  type: integer
- description: The collection the entity belongs to
  name: collectionId
  type: string
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-entity-schema.json
slug: microsoft-purview-entity
source_filename: microsoft-purview-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-entity-schema.json\",\n  \"title\": \"Microsoft Purview Atlas Entity\",\n  \"description\": \"Represents a data entity in the Microsoft Purview Data Map, based on the Apache Atlas entity model. Entities are the core building blocks of the data catalog.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attributes of the entity, defined by its type definition\",\n      \"additionalProperties\": true,\n      \"properties\": {\n        \"qualifiedName\": {\n          \"type\": \"string\",\n          \"description\": \"The unique qualified name of the entity\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the entity\"\n        },\n        \"description\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The description of the entity\"\n        },\n        \"owner\": {\n          \"type\": \"string\",\n          \"description\": \"The owner of the entity\"\n        }\n      }\n    },\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity type (e.g., azure_sql_table, azure_blob_path)\"\n    },\n    \"lastModifiedTS\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for concurrency control\"\n    },\n    \"businessAttributes\": {\n      \"type\": \"object\",\n      \"description\": \"Business metadata attributes attached to the entity\",\n      \"additionalProperties\": true\n    },\n    \"classifications\": {\n      \"type\": \"array\",\n      \"description\": \"Classifications applied to the entity\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AtlasClassification\"\n      }\n    },\n    \"createTime\": {\n      \"type\": \"integer\",\n      \"description\": \"The creation time of\
  \ the entity in epoch milliseconds\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the entity\"\n    },\n    \"guid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The globally unique identifier of the entity\"\n    },\n    \"homeId\": {\n      \"type\": \"string\",\n      \"description\": \"The home identifier\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the entity\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"meanings\": {\n      \"type\": \"array\",\n      \"description\": \"Glossary term assignments for the entity\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AtlasTermAssignmentHeader\"\n      }\n    },\n    \"provenanceType\": {\n      \"type\": \"integer\",\n      \"description\": \"The provenance type of the entity\"\n    },\n    \"proxy\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the entity is a proxy\"\n    },\n    \"relationshipAttributes\": {\n      \"type\": \"object\",\n      \"description\": \"Relationship attributes of the entity\",\n      \"additionalProperties\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the entity\",\n      \"enum\": [\"ACTIVE\", \"DELETED\"]\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"description\": \"The last update time of the entity in epoch milliseconds\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the entity\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number of the entity\"\n    },\n    \"collectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The collection the entity belongs to\"\n    }\n  },\n  \"required\": [\"typeName\"],\n  \"$defs\": {\n    \"AtlasClassification\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A classification applied to an entity\",\n      \"properties\": {\n        \"attributes\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"typeName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the classification type\"\n        },\n        \"lastModifiedTS\": {\n          \"type\": \"string\"\n        },\n        \"entityGuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"entityStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"ACTIVE\", \"DELETED\"]\n        },\n        \"propagate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the classification propagates to sub-entities\"\n        },\n        \"removePropagationsOnEntityDelete\": {\n          \"type\": \"boolean\"\n        },\n        \"validityPeriods\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"\
  type\": \"object\",\n            \"properties\": {\n              \"endTime\": { \"type\": \"string\" },\n              \"startTime\": { \"type\": \"string\" },\n              \"timeZone\": { \"type\": \"string\" }\n            }\n          }\n        }\n      },\n      \"required\": [\"typeName\"]\n    },\n    \"AtlasTermAssignmentHeader\": {\n      \"type\": \"object\",\n      \"description\": \"A glossary term assignment header\",\n      \"properties\": {\n        \"confidence\": {\n          \"type\": \"integer\"\n        },\n        \"createdBy\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"displayText\": {\n          \"type\": \"string\"\n        },\n        \"expression\": {\n          \"type\": \"string\"\n        },\n        \"relationGuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\"\
  : [\"DISCOVERED\", \"PROPOSED\", \"IMPORTED\", \"VALIDATED\", \"DEPRECATED\", \"OBSOLETE\", \"OTHER\"]\n        },\n        \"steward\": {\n          \"type\": \"string\"\n        },\n        \"termGuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-entity-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Atlas Entity
---
