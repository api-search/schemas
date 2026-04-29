---
description: Describes a snapshot.
layout: schema
name: Snapshot
properties_list:
- description: ''
  name: SnapshotTime
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-snapshot-schema.json
slug: workspaces-snapshot
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the snapshot was created.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a snapshot.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Snapshot\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-snapshot-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-snapshot-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: Snapshot
---
