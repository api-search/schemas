---
description: DescribeWorkspaceSnapshotsRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceSnapshotsRequest
properties_list:
- description: ''
  name: WorkspaceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-snapshots-request-schema.json
slug: workspaces-describe-workspace-snapshots-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"WorkspaceId\"\n  ],\n  \"title\": \"DescribeWorkspaceSnapshotsRequest\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-snapshots-request-schema.json\",\n  \"description\": \"DescribeWorkspaceSnapshotsRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-snapshots-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceSnapshotsRequest
---
