---
description: CreateSnapshotInput schema from Amazon SimSpace Weaver API
layout: schema
name: CreateSnapshotInput
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: Simulation
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-create-snapshot-input-schema.json
slug: amazon-simspace-weaver-create-snapshot-input
source_filename: amazon-simspace-weaver-create-snapshot-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-create-snapshot-input-schema.json\",\n  \"title\": \"CreateSnapshotInput\",\n  \"description\": \"CreateSnapshotInput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 bucket and optional folder (object key prefix) where SimSpace Weaver creates the snapshot file.</p> <p>The Amazon S3 bucket must be in the same Amazon Web Services Region as the simulation.</p>\"\n        }\n      ]\n    },\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\"\
  : \"The name of the simulation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\",\n    \"Simulation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-create-snapshot-input-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: CreateSnapshotInput
---
