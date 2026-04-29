---
description: UpdateRulesOfIpGroupRequest schema from Amazon WorkSpaces API
layout: schema
name: UpdateRulesOfIpGroupRequest
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: UserRules
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-update-rules-of-ip-group-request-schema.json
slug: workspaces-update-rules-of-ip-group-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupId\",\n    \"UserRules\"\n  ],\n  \"title\": \"UpdateRulesOfIpGroupRequest\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    },\n    \"UserRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleList\"\n        },\n        {\n          \"description\": \"One or more rules.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-rules-of-ip-group-request-schema.json\",\n  \"description\": \"UpdateRulesOfIpGroupRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-update-rules-of-ip-group-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: UpdateRulesOfIpGroupRequest
---
