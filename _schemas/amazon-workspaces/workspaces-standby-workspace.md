---
description: Describes a standby WorkSpace.
layout: schema
name: StandbyWorkspace
properties_list:
- description: ''
  name: PrimaryWorkspaceId
  type: object
- description: ''
  name: VolumeEncryptionKey
  type: object
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-standby-workspace-schema.json
slug: workspaces-standby-workspace
source_filename: workspaces-standby-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"PrimaryWorkspaceId\",\n    \"DirectoryId\"\n  ],\n  \"properties\": {\n    \"PrimaryWorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the standby WorkSpace.\"\n        }\n      ]\n    },\n    \"VolumeEncryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeEncryptionKey\"\n        },\n        {\n          \"description\": \"The volume encryption key of the standby WorkSpace.\"\n        }\n      ]\n    },\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory for the standby WorkSpace.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n\
  \        },\n        {\n          \"description\": \"The tags associated with the standby WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a standby WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StandbyWorkspace\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-standby-workspace-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-standby-workspace-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: StandbyWorkspace
---
