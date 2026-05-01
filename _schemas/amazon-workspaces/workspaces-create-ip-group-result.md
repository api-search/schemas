---
description: CreateIpGroupResult schema from Amazon WorkSpaces API
layout: schema
name: CreateIpGroupResult
properties_list:
- description: ''
  name: GroupId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-ip-group-result-schema.json
slug: workspaces-create-ip-group-result
source_filename: workspaces-create-ip-group-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateIpGroupResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-ip-group-result-schema.json\",\n  \"description\": \"CreateIpGroupResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-ip-group-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateIpGroupResult
---
