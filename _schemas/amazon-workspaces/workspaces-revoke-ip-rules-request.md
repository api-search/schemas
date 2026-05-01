---
description: RevokeIpRulesRequest schema from Amazon WorkSpaces API
layout: schema
name: RevokeIpRulesRequest
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: UserRules
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-revoke-ip-rules-request-schema.json
slug: workspaces-revoke-ip-rules-request
source_filename: workspaces-revoke-ip-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupId\",\n    \"UserRules\"\n  ],\n  \"title\": \"RevokeIpRulesRequest\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    },\n    \"UserRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRevokedRuleList\"\n        },\n        {\n          \"description\": \"The rules to remove from the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-revoke-ip-rules-request-schema.json\",\n  \"description\": \"RevokeIpRulesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-revoke-ip-rules-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RevokeIpRulesRequest
---
