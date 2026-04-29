---
description: Configurations for a single stream.
layout: schema
name: StreamConfiguration
properties_list:
- description: ''
  name: name
  type: string
- description: Namespace of the stream.
  name: namespace
  type: string
- description: ''
  name: syncMode
  type: object
- description: Path to the field that will be used to determine if a record is new or modified since the last sync. This field is REQUIRED if `sync_mode` is `incremental` unless there is a default.
  name: cursorField
  type: array
- description: Paths to the fields that will be used as primary key. This field is REQUIRED if `destination_sync_mode` is `*_dedup` unless it is already supplied by the source schema.
  name: primaryKey
  type: array
- description: Whether to move raw files from the source to the destination during the sync.
  name: includeFiles
  type: boolean
- description: The name of the destination object that this stream will be written to, used for data activation destinations.
  name: destinationObjectName
  type: string
- description: By default (if not provided in the request) all fields will be synced. Otherwise, only the fields in this list will be synced.
  name: selectedFields
  type: object
- description: Mappers that should be applied to the stream before writing to the destination.
  name: mappers
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-stream-configuration-schema.json
slug: airbyte-stream-configuration
source_filename: airbyte-stream-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-configuration-schema.json\",\n  \"title\": \"StreamConfiguration\",\n  \"description\": \"Configurations for a single stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Namespace of the stream.\"\n    },\n    \"syncMode\": {\n      \"$ref\": \"#/components/schemas/ConnectionSyncModeEnum\"\n    },\n    \"cursorField\": {\n      \"description\": \"Path to the field that will be used to determine if a record is new or modified since the last sync. This field is REQUIRED if `sync_mode` is `incremental` unless there is a default.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"primaryKey\": {\n      \"description\"\
  : \"Paths to the fields that will be used as primary key. This field is REQUIRED if `destination_sync_mode` is `*_dedup` unless it is already supplied by the source schema.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"includeFiles\": {\n      \"description\": \"Whether to move raw files from the source to the destination during the sync.\",\n      \"type\": \"boolean\"\n    },\n    \"destinationObjectName\": {\n      \"description\": \"The name of the destination object that this stream will be written to, used for data activation destinations.\",\n      \"type\": \"string\"\n    },\n    \"selectedFields\": {\n      \"description\": \"By default (if not provided in the request) all fields will be synced. Otherwise, only the fields in this list will be synced.\",\n      \"$ref\": \"#/components/schemas/SelectedFields\"\n    },\n    \"mappers\": {\n      \"description\"\
  : \"Mappers that should be applied to the stream before writing to the destination.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConfiguredStreamMapper\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-stream-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: StreamConfiguration
---
