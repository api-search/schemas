---
description: CreateStandbyWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateStandbyWorkspacesRequest
properties_list:
- description: ''
  name: PrimaryRegion
  type: object
- description: ''
  name: StandbyWorkspaces
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-standby-workspaces-request-schema.json
slug: workspaces-create-standby-workspaces-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"PrimaryRegion\",\n    \"StandbyWorkspaces\"\n  ],\n  \"title\": \"CreateStandbyWorkspacesRequest\",\n  \"properties\": {\n    \"PrimaryRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Region of the primary WorkSpace.\"\n        }\n      ]\n    },\n    \"StandbyWorkspaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StandbyWorkspacesList\"\n        },\n        {\n          \"description\": \"Information about the standby WorkSpace to be created.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-standby-workspaces-request-schema.json\",\n  \"description\": \"CreateStandbyWorkspacesRequest schema from Amazon WorkSpaces\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-standby-workspaces-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateStandbyWorkspacesRequest
---
