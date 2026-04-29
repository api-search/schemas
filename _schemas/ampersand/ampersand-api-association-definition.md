---
description: Relationship information for a field to another object
layout: schema
name: AssociationDefinition
properties_list:
- description: High-level association variety (e.g., 'foreignKey', 'lookup', 'ref')
  name: associationType
  type: string
- description: Name of the referenced/parent object
  name: targetObject
  type: string
- description: Name of the referenced field on the target object
  name: targetField
  type: string
- description: Association cardinality from the referencing field's perspective
  name: cardinality
  type: string
- description: Behavior upon foreign object deletion
  name: onDelete
  type: string
- description: If true, a referenced record must exist
  name: required
  type: boolean
- description: Optional inverse relationship/property name exposed on the target object
  name: reverseLookupFieldName
  type: string
- description: ''
  name: labels
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-association-definition-schema.json
slug: ampersand-api-association-definition
source_filename: ampersand-api-association-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-association-definition-schema.json\",\n  \"title\": \"AssociationDefinition\",\n  \"description\": \"Relationship information for a field to another object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associationType\": {\n      \"type\": \"string\",\n      \"description\": \"High-level association variety (e.g., 'foreignKey', 'lookup', 'ref')\",\n      \"example\": \"foreignKey\"\n    },\n    \"targetObject\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the referenced/parent object\",\n      \"example\": \"Account\"\n    },\n    \"targetField\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the referenced field on the target object\"\n    },\n    \"cardinality\": {\n      \"type\": \"string\",\n      \"description\": \"Association cardinality\
  \ from the referencing field's perspective\",\n      \"example\": \"many-to-one\"\n    },\n    \"onDelete\": {\n      \"type\": \"string\",\n      \"description\": \"Behavior upon foreign object deletion\",\n      \"example\": \"setNull\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, a referenced record must exist\"\n    },\n    \"reverseLookupFieldName\": {\n      \"type\": \"string\",\n      \"description\": \"Optional inverse relationship/property name exposed on the target object\"\n    },\n    \"labels\": {\n      \"$ref\": \"#/components/schemas/AssociationLabels\"\n    }\n  },\n  \"required\": [\n    \"associationType\",\n    \"targetObject\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-association-definition-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: AssociationDefinition
---
