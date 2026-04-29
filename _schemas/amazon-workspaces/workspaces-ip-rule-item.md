---
description: Describes a rule for an IP access control group.
layout: schema
name: IpRuleItem
properties_list:
- description: ''
  name: ipRule
  type: object
- description: ''
  name: ruleDesc
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-ip-rule-item-schema.json
slug: workspaces-ip-rule-item
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRule\"\n        },\n        {\n          \"description\": \"The IP address range, in CIDR notation.\"\n        }\n      ]\n    },\n    \"ruleDesc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleDesc\"\n        },\n        {\n          \"description\": \"The description.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a rule for an IP access control group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpRuleItem\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-ip-rule-item-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-ip-rule-item-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: IpRuleItem
---
