---
description: Metadata definition for a Dataverse table (entity). Provides information about the table structure including logical names, collection names, and configuration. Read-only entity type supporting only RetrieveMultiple operations.
layout: schema
name: Entity
properties_list:
- description: Unique identifier of the entity definition.
  name: entityid
  type: string
- description: Display name of the entity.
  name: name
  type: string
- description: Logical name of the entity, used in API requests and programmatic references.
  name: logicalname
  type: string
- description: Logical collection name of the entity.
  name: logicalcollectionname
  type: string
- description: Collection name of the entity.
  name: collectionname
  type: string
- description: Entity set name used in Web API URLs to reference this table.
  name: entitysetname
  type: string
- description: Physical database table name of the entity.
  name: physicalname
  type: string
- description: Base table name of the entity.
  name: basetablename
  type: string
- description: External name of the entity for virtual entities.
  name: externalname
  type: string
- description: External collection name of the entity.
  name: externalcollectionname
  type: string
- description: Address table name associated with the entity.
  name: addresstablename
  type: string
- description: Extension table name of the entity.
  name: extensiontablename
  type: string
- description: Report view name of the entity.
  name: reportviewname
  type: string
- description: Parent controlling attribute name of the entity.
  name: parentcontrollingattributename
  type: string
- description: Original localized display name of the entity.
  name: originallocalizedname
  type: string
- description: Original localized collection name of the entity.
  name: originallocalizedcollectionname
  type: string
- description: Whether this entity is an activity type.
  name: isactivity
  type: boolean
- description: Object type code of the entity.
  name: objecttypecode
  type: integer
- description: Component state of the entity. 0 = Published, 1 = Unpublished, 2 = Deleted, 3 = Deleted Unpublished.
  name: componentstate
  type: integer
- description: Unique identifier of the associated solution.
  name: solutionid
  type: string
- description: Record overwrite time for internal use.
  name: overwritetime
  type: string
- description: Version number of the entity definition record.
  name: versionnumber
  type: integer
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
schema_file: json-schema/microsoft-power-apps-dataverse-web-entity-schema.json
slug: microsoft-power-apps-dataverse-web-entity
source_filename: microsoft-power-apps-dataverse-web-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Entity\",\n  \"type\": \"object\",\n  \"description\": \"Metadata definition for a Dataverse table (entity). Provides information about the table structure including logical names, collection names, and configuration. Read-only entity type supporting only RetrieveMultiple operations.\",\n  \"properties\": {\n    \"entityid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the entity definition.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the entity.\"\n    },\n    \"logicalname\": {\n      \"type\": \"string\",\n      \"description\": \"Logical name of the entity, used in API requests and programmatic references.\"\n    },\n    \"logicalcollectionname\": {\n      \"type\": \"string\",\n      \"description\": \"Logical collection name of the entity.\"\n    },\n    \"collectionname\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Collection name of the entity.\"\n    },\n    \"entitysetname\": {\n      \"type\": \"string\",\n      \"description\": \"Entity set name used in Web API URLs to reference this table.\"\n    },\n    \"physicalname\": {\n      \"type\": \"string\",\n      \"description\": \"Physical database table name of the entity.\"\n    },\n    \"basetablename\": {\n      \"type\": \"string\",\n      \"description\": \"Base table name of the entity.\"\n    },\n    \"externalname\": {\n      \"type\": \"string\",\n      \"description\": \"External name of the entity for virtual entities.\"\n    },\n    \"externalcollectionname\": {\n      \"type\": \"string\",\n      \"description\": \"External collection name of the entity.\"\n    },\n    \"addresstablename\": {\n      \"type\": \"string\",\n      \"description\": \"Address table name associated with the entity.\"\n    },\n    \"extensiontablename\": {\n      \"type\": \"string\",\n      \"description\": \"Extension table\
  \ name of the entity.\"\n    },\n    \"reportviewname\": {\n      \"type\": \"string\",\n      \"description\": \"Report view name of the entity.\"\n    },\n    \"parentcontrollingattributename\": {\n      \"type\": \"string\",\n      \"description\": \"Parent controlling attribute name of the entity.\"\n    },\n    \"originallocalizedname\": {\n      \"type\": \"string\",\n      \"description\": \"Original localized display name of the entity.\"\n    },\n    \"originallocalizedcollectionname\": {\n      \"type\": \"string\",\n      \"description\": \"Original localized collection name of the entity.\"\n    },\n    \"isactivity\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this entity is an activity type.\"\n    },\n    \"objecttypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Object type code of the entity.\"\n    },\n    \"componentstate\": {\n      \"type\": \"integer\",\n      \"description\": \"Component state of the entity. 0 = Published,\
  \ 1 = Unpublished, 2 = Deleted, 3 = Deleted Unpublished.\"\n    },\n    \"solutionid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the associated solution.\"\n    },\n    \"overwritetime\": {\n      \"type\": \"string\",\n      \"description\": \"Record overwrite time for internal use.\"\n    },\n    \"versionnumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the entity definition record.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/json-schema/microsoft-power-apps-dataverse-web-entity-schema.json
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
title: Entity
---
