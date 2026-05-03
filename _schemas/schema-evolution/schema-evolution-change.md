---
description: Represents a single change made to a data schema between versions, including its type, scope, and compatibility impact.
layout: schema
name: Schema Change
properties_list:
- description: Unique identifier for this change record
  name: id
  type: string
- description: Name of the schema being changed
  name: schemaName
  type: string
- description: Version number before this change
  name: fromVersion
  type: string
- description: Version number after this change
  name: toVersion
  type: string
- description: Type of schema change made
  name: changeType
  type: string
- description: JSON path to the field affected by this change (e.g., 'properties.user.email')
  name: fieldPath
  type: string
- description: How this change affects schema compatibility
  name: compatibilityImpact
  type: string
- description: Human-readable description of the change and its rationale
  name: description
  type: string
- description: Whether data migration is required for existing records
  name: migrationRequired
  type: boolean
- description: SQL, migration script, or transformation logic description
  name: migrationScript
  type: string
- description: Date when the change was applied
  name: date
  type: string
- description: Person or team responsible for the change
  name: author
  type: string
provider_name: Schema Evolution
provider_slug: schema-evolution
schema_file: json-schema/schema-evolution-change-schema.json
slug: schema-evolution-change
source_filename: schema-evolution-change-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/schema-evolution/blob/main/json-schema/schema-evolution-change-schema.json\",\n  \"title\": \"Schema Change\",\n  \"description\": \"Represents a single change made to a data schema between versions, including its type, scope, and compatibility impact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this change record\"\n    },\n    \"schemaName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schema being changed\"\n    },\n    \"fromVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version number before this change\"\n    },\n    \"toVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version number after this change\"\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Type of schema change made\",\n      \"enum\": [\n        \"field-added\",\n        \"field-removed\",\n        \"field-renamed\",\n        \"field-type-changed\",\n        \"field-made-required\",\n        \"field-made-optional\",\n        \"field-default-added\",\n        \"field-default-changed\",\n        \"enum-value-added\",\n        \"enum-value-removed\",\n        \"schema-created\",\n        \"schema-deprecated\",\n        \"schema-removed\",\n        \"constraint-added\",\n        \"constraint-removed\"\n      ]\n    },\n    \"fieldPath\": {\n      \"type\": \"string\",\n      \"description\": \"JSON path to the field affected by this change (e.g., 'properties.user.email')\"\n    },\n    \"compatibilityImpact\": {\n      \"type\": \"string\",\n      \"description\": \"How this change affects schema compatibility\",\n      \"enum\": [\"backward-compatible\", \"forward-compatible\", \"fully-compatible\", \"breaking\"]\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Human-readable description of the change and its rationale\"\n    },\n    \"migrationRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether data migration is required for existing records\"\n    },\n    \"migrationScript\": {\n      \"type\": \"string\",\n      \"description\": \"SQL, migration script, or transformation logic description\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the change was applied\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Person or team responsible for the change\"\n    }\n  },\n  \"required\": [\"schemaName\", \"fromVersion\", \"toVersion\", \"changeType\", \"compatibilityImpact\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-evolution/refs/heads/main/json-schema/schema-evolution-change-schema.json
tags:
- Schema Evolution
- Backward Compatibility
- Forward Compatibility
- API Versioning
- Breaking Changes
- Schema Registry
- Data Migration
- Kafka
title: Schema Change
---
