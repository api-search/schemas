---
description: A Changelog Entry records a schema change in a federated graph's composition history.
layout: schema
name: WunderGraph Cosmo Changelog Entry
properties_list:
- description: Unique identifier for the changelog entry.
  name: id
  type: string
- description: The schema version associated with this change.
  name: schemaVersionId
  type: string
- description: When the change occurred.
  name: createdAt
  type: string
- description: The type of schema change.
  name: changeType
  type: string
- description: The schema path that changed.
  name: path
  type: string
- description: Description of the change.
  name: changeMessage
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/changelog-entry.json
slug: changelog-entry
source_filename: changelog-entry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/changelog-entry.json\",\n  \"title\": \"WunderGraph Cosmo Changelog Entry\",\n  \"description\": \"A Changelog Entry records a schema change in a federated graph's composition history.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the changelog entry.\"\n    },\n    \"schemaVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The schema version associated with this change.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the change occurred.\"\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of schema change.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The schema\
  \ path that changed.\"\n    },\n    \"changeMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the change.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/changelog-entry.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Changelog Entry
---
