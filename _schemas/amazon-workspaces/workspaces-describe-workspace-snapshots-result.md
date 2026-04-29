---
description: DescribeWorkspaceSnapshotsResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceSnapshotsResult
properties_list:
- description: ''
  name: RebuildSnapshots
  type: object
- description: ''
  name: RestoreSnapshots
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-snapshots-result-schema.json
slug: workspaces-describe-workspace-snapshots-result
source_filename: workspaces-describe-workspace-snapshots-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RebuildSnapshots\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotList\"\n        },\n        {\n          \"description\": \"Information about the snapshots that can be used to rebuild a WorkSpace. These snapshots include the user volume.\"\n        }\n      ]\n    },\n    \"RestoreSnapshots\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotList\"\n        },\n        {\n          \"description\": \"Information about the snapshots that can be used to restore a WorkSpace. These snapshots include both the root volume and the user volume.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeWorkspaceSnapshotsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-snapshots-result-schema.json\"\
  ,\n  \"description\": \"DescribeWorkspaceSnapshotsResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-snapshots-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceSnapshotsResult
---
