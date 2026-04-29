---
description: Unit status.
layout: schema
name: UnitStatus
properties_list:
- description: Unit identifier.
  name: id
  type: string
- description: Map from unit version to unit deployment status.
  name: versionToStatus
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-unit-status-schema.json
slug: rest-api-unit-status
source_filename: rest-api-unit-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-unit-status-schema.json\",\n  \"title\": \"UnitStatus\",\n  \"description\": \"Unit status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unit identifier.\"\n    },\n    \"versionToStatus\": {\n      \"type\": \"array\",\n      \"description\": \"Map from unit version to unit deployment status.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UnitVersionStatus\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"versionToStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-unit-status-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: UnitStatus
---
