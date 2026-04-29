---
description: Metadata common to all entity kinds.
layout: schema
name: EntityMetadata
properties_list:
- description: A globally unique identifier for the entity.
  name: uid
  type: string
- description: An opaque string that changes on each update.
  name: etag
  type: string
- description: The name of the entity.
  name: name
  type: string
- description: The namespace the entity belongs to.
  name: namespace
  type: string
- description: A human-readable title for the entity.
  name: title
  type: string
- description: A human-readable description of the entity.
  name: description
  type: string
- description: Key-value pairs for labeling the entity.
  name: labels
  type: object
- description: Key-value pairs for non-identifying metadata.
  name: annotations
  type: object
- description: A list of single-valued strings for classification.
  name: tags
  type: array
- description: ''
  name: links
  type: array
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/catalog-entity-metadata-schema.json
slug: catalog-entity-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-metadata-schema.json\",\n  \"title\": \"EntityMetadata\",\n  \"description\": \"Metadata common to all entity kinds.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"A globally unique identifier for the entity.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque string that changes on each update.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity.\",\n      \"example\": \"my-service\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace the entity belongs to.\",\n      \"default\": \"default\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"\
  description\": \"A human-readable title for the entity.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the entity.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for labeling the entity.\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for non-identifying metadata.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of single-valued strings for classification.\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\"\
  : \"uri\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          },\n          \"icon\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/catalog-entity-metadata-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: EntityMetadata
---
