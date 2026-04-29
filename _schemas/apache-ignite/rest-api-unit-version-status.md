---
description: Unit version and status.
layout: schema
name: UnitVersionStatus
properties_list:
- description: Unit version.
  name: version
  type: string
- description: ''
  name: status
  type: object
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-unit-version-status-schema.json
slug: rest-api-unit-version-status
source_filename: rest-api-unit-version-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-unit-version-status-schema.json\",\n  \"title\": \"UnitVersionStatus\",\n  \"description\": \"Unit version and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Unit version.\"\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"Unit status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/json-schema/rest-api-unit-version-status-schema.json
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: UnitVersionStatus
---
