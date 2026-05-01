---
description: The summary of IP access settings.
layout: schema
name: IpAccessSettingsSummary
properties_list:
- description: ''
  name: creationDate
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: ipAccessSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-ip-access-settings-summary-schema.json
slug: workspaces-web-ip-access-settings-summary
source_filename: workspaces-web-ip-access-settings-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date timestamp of the IP access settings.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the IP access settings.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The display name of the IP access settings.\"\n        }\n      ]\n    },\n    \"ipAccessSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of IP access settings.\"\n        }\n\
  \      ]\n    }\n  },\n  \"description\": \"The summary of IP access settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpAccessSettingsSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-access-settings-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-access-settings-summary-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IpAccessSettingsSummary
---
