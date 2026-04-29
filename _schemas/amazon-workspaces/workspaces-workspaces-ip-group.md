---
description: Describes an IP access control group.
layout: schema
name: WorkspacesIpGroup
properties_list:
- description: ''
  name: groupId
  type: object
- description: ''
  name: groupName
  type: object
- description: ''
  name: groupDesc
  type: object
- description: ''
  name: userRules
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspaces-ip-group-schema.json
slug: workspaces-workspaces-ip-group
source_filename: workspaces-workspaces-ip-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    },\n    \"groupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupName\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"groupDesc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupDesc\"\n        },\n        {\n          \"description\": \"The description of the group.\"\n        }\n      ]\n    },\n    \"userRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleList\"\n        },\n        {\n          \"description\": \"The rules.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes an IP access control group.\",\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspacesIpGroup\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspaces-ip-group-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspaces-ip-group-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspacesIpGroup
---
