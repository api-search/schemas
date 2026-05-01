---
description: The summary of user access logging settings.
layout: schema
name: UserAccessLoggingSettingsSummary
properties_list:
- description: ''
  name: kinesisStreamArn
  type: object
- description: ''
  name: userAccessLoggingSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-user-access-logging-settings-summary-schema.json
slug: workspaces-web-user-access-logging-settings-summary
source_filename: workspaces-web-user-access-logging-settings-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"kinesisStreamArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamArn\"\n        },\n        {\n          \"description\": \"The ARN of the Kinesis stream.\"\n        }\n      ]\n    },\n    \"userAccessLoggingSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user access logging settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of user access logging settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAccessLoggingSettingsSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-access-logging-settings-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-access-logging-settings-summary-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UserAccessLoggingSettingsSummary
---
