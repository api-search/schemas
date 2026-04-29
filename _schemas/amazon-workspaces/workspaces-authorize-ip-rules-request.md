---
description: AuthorizeIpRulesRequest schema from Amazon WorkSpaces API
layout: schema
name: AuthorizeIpRulesRequest
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: UserRules
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-authorize-ip-rules-request-schema.json
slug: workspaces-authorize-ip-rules-request
source_filename: workspaces-authorize-ip-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupId\",\n    \"UserRules\"\n  ],\n  \"title\": \"AuthorizeIpRulesRequest\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the group.\"\n        }\n      ]\n    },\n    \"UserRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleList\"\n        },\n        {\n          \"description\": \"The rules to add to the group.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-authorize-ip-rules-request-schema.json\",\n  \"description\": \"AuthorizeIpRulesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-authorize-ip-rules-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: AuthorizeIpRulesRequest
---
