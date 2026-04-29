---
description: The summary of user settings.
layout: schema
name: UserSettingsSummary
properties_list:
- description: ''
  name: copyAllowed
  type: object
- description: ''
  name: disconnectTimeoutInMinutes
  type: object
- description: ''
  name: downloadAllowed
  type: object
- description: ''
  name: idleDisconnectTimeoutInMinutes
  type: object
- description: ''
  name: pasteAllowed
  type: object
- description: ''
  name: printAllowed
  type: object
- description: ''
  name: uploadAllowed
  type: object
- description: ''
  name: userSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-user-settings-summary-schema.json
slug: workspaces-web-user-settings-summary
source_filename: workspaces-web-user-settings-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"copyAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledType\"\n        },\n        {\n          \"description\": \"Specifies whether the user can copy text from the streaming session to the local device.\"\n        }\n      ]\n    },\n    \"disconnectTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisconnectTimeoutInMinutes\"\n        },\n        {\n          \"description\": \"The amount of time that a streaming session remains active after users disconnect.\"\n        }\n      ]\n    },\n    \"downloadAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledType\"\n        },\n        {\n          \"description\": \"Specifies whether the user can download files from the streaming session to the local device.\"\n        }\n      ]\n    },\n    \"idleDisconnectTimeoutInMinutes\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdleDisconnectTimeoutInMinutes\"\n        },\n        {\n          \"description\": \"The amount of time that users can be idle (inactive) before they are disconnected from their streaming session and the disconnect timeout interval begins.\"\n        }\n      ]\n    },\n    \"pasteAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledType\"\n        },\n        {\n          \"description\": \"Specifies whether the user can paste text from the local device to the streaming session.\"\n        }\n      ]\n    },\n    \"printAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledType\"\n        },\n        {\n          \"description\": \"Specifies whether the user can print to the local device.\"\n        }\n      ]\n    },\n    \"uploadAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledType\"\n    \
  \    },\n        {\n          \"description\": \"Specifies whether the user can upload files from the local device to the streaming session.\"\n        }\n      ]\n    },\n    \"userSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of user settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserSettingsSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-settings-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-user-settings-summary-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UserSettingsSummary
---
