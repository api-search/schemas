---
description: CreateIpGroupRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateIpGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: GroupDesc
  type: object
- description: ''
  name: UserRules
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-ip-group-request-schema.json
slug: workspaces-create-ip-group-request
source_filename: workspaces-create-ip-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupName\"\n  ],\n  \"title\": \"CreateIpGroupRequest\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupName\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"GroupDesc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupDesc\"\n        },\n        {\n          \"description\": \"The description of the group.\"\n        }\n      ]\n    },\n    \"UserRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleList\"\n        },\n        {\n          \"description\": \"The rules to add to the group.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags. Each WorkSpaces resource can\
  \ have a maximum of 50 tags.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-ip-group-request-schema.json\",\n  \"description\": \"CreateIpGroupRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-ip-group-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateIpGroupRequest
---
