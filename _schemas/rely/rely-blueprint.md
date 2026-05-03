---
description: A blueprint schema defining the structure and attributes of a catalog entity type in Rely.io
layout: schema
name: Rely.io Blueprint
properties_list:
- description: Globally unique blueprint identifier
  name: id
  type: string
- description: User-friendly display name for the blueprint
  name: name
  type: string
- description: Optional overview of what this blueprint represents
  name: description
  type:
  - string
  - 'null'
- description: Schema definitions for properties of entities of this type
  name: properties
  type: object
- description: Relation definitions linking this blueprint to other blueprint types
  name: relations
  type: object
- description: Blueprint creation timestamp
  name: createdAt
  type: string
- description: Blueprint last update timestamp
  name: updatedAt
  type: string
provider_name: Rely.io
provider_slug: rely
schema_file: json-schema/rely-blueprint-schema.json
slug: rely-blueprint
source_filename: rely-blueprint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rely/json-schema/rely-blueprint-schema.json\",\n  \"title\": \"Rely.io Blueprint\",\n  \"description\": \"A blueprint schema defining the structure and attributes of a catalog entity type in Rely.io\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique blueprint identifier\",\n      \"pattern\": \"^[a-z][a-z0-9-_]*$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly display name for the blueprint\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional overview of what this blueprint represents\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Schema definitions for properties of entities of this type\",\n      \"additionalProperties\"\
  : {\n        \"$ref\": \"#/$defs/BlueprintProperty\"\n      }\n    },\n    \"relations\": {\n      \"type\": \"object\",\n      \"description\": \"Relation definitions linking this blueprint to other blueprint types\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/BlueprintRelation\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Blueprint creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Blueprint last update timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"BlueprintProperty\": {\n      \"type\": \"object\",\n      \"description\": \"A property definition within a blueprint schema\",\n      \"required\": [\"title\", \"type\"],\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Display name for the property\"\n        },\n        \"type\": {\n\
  \          \"type\": \"string\",\n          \"enum\": [\"string\", \"integer\", \"number\", \"boolean\", \"array\", \"object\"],\n          \"description\": \"JSON Schema data type\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the property's purpose\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"JSON Schema format (date-time, uri, email, etc.)\"\n        },\n        \"enum\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed values for enum properties\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this property is required on entities\"\n        }\n      }\n    },\n    \"BlueprintRelation\": {\n      \"type\": \"object\",\n      \"description\": \"A relation linking this blueprint to another blueprint type\",\n      \"required\": [\"title\", \"target\"],\n      \"properties\"\
  : {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Display name for the relation\"\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"Target blueprint identifier\"\n        },\n        \"many\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a one-to-many relation\",\n          \"default\": false\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the relation\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rely/refs/heads/main/json-schema/rely-blueprint-schema.json
tags:
- Developer Experience
- Internal Developer Portal
- Platform Engineering
- Software Catalog
- Service Catalog
- Engineering Scorecards
title: Rely.io Blueprint
---
