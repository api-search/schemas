---
description: A user access logging settings resource that can be associated with a web portal.
layout: schema
name: UserAccessLoggingSettings
properties_list:
- description: ''
  name: associatedPortalArns
  type: object
- description: ''
  name: kinesisStreamArn
  type: object
- description: ''
  name: userAccessLoggingSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-user-access-logging-settings-schema.json
slug: workspaces-web-user-access-logging-settings
source_filename: workspaces-web-user-access-logging-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"userAccessLoggingSettingsArn\"\n  ],\n  \"properties\": {\n    \"associatedPortalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"A list of web portal ARNs that this user access logging settings is associated with.\"\n        }\n      ]\n    },\n    \"kinesisStreamArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamArn\"\n        },\n        {\n          \"description\": \"The ARN of the Kinesis stream.\"\n        }\n      ]\n    },\n    \"userAccessLoggingSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user access logging settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A user access logging settings resource that can be associated with a web portal.\"\
  ,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserAccessLoggingSettings\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-access-logging-settings-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-access-logging-settings-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UserAccessLoggingSettings
---
