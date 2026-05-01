---
description: A reported observation event for an external asset in Dagster.
layout: schema
name: AssetObservation
properties_list:
- description: The asset key being observed.
  name: asset_key
  type: string
- description: Free-form key/value metadata about the observation.
  name: metadata
  type: object
- description: A user-supplied data version identifier.
  name: data_version
  type: string
- description: A human-readable description of the observation.
  name: description
  type: string
- description: The asset partition associated with the observation.
  name: partition
  type: string
provider_name: Dagster
provider_slug: dagster
schema_file: json-schema/asset-observation.json
slug: asset-observation
source_filename: asset-observation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/json-schema/asset-observation.json\",\n  \"title\": \"AssetObservation\",\n  \"description\": \"A reported observation event for an external asset in Dagster.\",\n  \"type\": \"object\",\n  \"required\": [\"asset_key\"],\n  \"properties\": {\n    \"asset_key\": {\n      \"type\": \"string\",\n      \"description\": \"The asset key being observed.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Free-form key/value metadata about the observation.\",\n      \"additionalProperties\": true\n    },\n    \"data_version\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied data version identifier.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the observation.\"\n    },\n    \"partition\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The asset partition associated with the observation.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/json-schema/asset-observation.json
tags:
- Data Engineering
- Data Orchestration
- Data Pipelines
- ETL
- Workflows
- Assets
- GraphQL
title: AssetObservation
---
