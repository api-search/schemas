---
description: ''
layout: schema
name: IngestionJob
properties_list:
- description: Indicate if data described in source uri shall be deleted after ingestion. Source uri must be a cloud storage uri. If deletion failed, ingestion status is set to `FAILED`.
  name: deleteOrigin
  type: boolean
- description: Indicate if data described in source uri shall be copied for archive after ingestion. If copy failed, ingestion status is set to `FAILED`.
  name: nativeCopy
  type: boolean
- description: Uri of the resource to ingest. The uri must point to the main file of the resource.
  name: sourceUri
  type: string
- description: Type of data to ingest
  name: type
  type: string
- description: ''
  name: workspace
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-ingestion-job-schema.json
slug: oneatlas-ingestion-job
source_filename: oneatlas-ingestion-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-ingestion-job-schema.json\",\n  \"title\": \"IngestionJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deleteOrigin\": {\n      \"default\": false,\n      \"description\": \"Indicate if data described in source uri shall be deleted after ingestion. Source uri must be a cloud storage uri. If deletion failed, ingestion status is set to `FAILED`.\",\n      \"type\": \"boolean\"\n    },\n    \"nativeCopy\": {\n      \"default\": false,\n      \"description\": \"Indicate if data described in source uri shall be copied for archive after ingestion. If copy failed, ingestion status is set to `FAILED`.\",\n      \"type\": \"boolean\"\n    },\n    \"sourceUri\": {\n      \"description\": \"Uri of the resource to ingest. The uri must point to the main file of the resource.\",\n      \"example\"\
  : \"gs://gcp-public-data-sentinel-2/tiles/28/R/DP/S2A_MSIL1C_20171224T113501_N0206_R080_T28RDP_20171224T133237.SAFE\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of data to ingest\",\n      \"enum\": [\n        \"changeDetectionReport\",\n        \"oceanWayReport\",\n        \"pleiades\",\n        \"sentinel2\",\n        \"spot\",\n        \"vectorFile\"\n      ],\n      \"example\": \"sentinel2\",\n      \"type\": \"string\"\n    },\n    \"workspace\": {\n      \"$ref\": \"#/components/schemas/WorkspaceIdentifier\"\n    }\n  },\n  \"required\": [\n    \"workspace\",\n    \"sourceUri\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-ingestion-job-schema.json
tags:
- Imagery
- Satellites
title: IngestionJob
---
