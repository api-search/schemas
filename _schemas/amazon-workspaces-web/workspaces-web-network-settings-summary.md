---
description: The summary of network settings.
layout: schema
name: NetworkSettingsSummary
properties_list:
- description: ''
  name: networkSettingsArn
  type: object
- description: ''
  name: vpcId
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-network-settings-summary-schema.json
slug: workspaces-web-network-settings-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the network settings.\"\n        }\n      ]\n    },\n    \"vpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcId\"\n        },\n        {\n          \"description\": \"The VPC ID of the network settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of network settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkSettingsSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-network-settings-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-network-settings-summary-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: NetworkSettingsSummary
---
