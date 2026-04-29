---
description: Describes an Amazon WorkSpaces client.
layout: schema
name: ClientProperties
properties_list:
- description: ''
  name: ReconnectEnabled
  type: object
- description: ''
  name: LogUploadEnabled
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-client-properties-schema.json
slug: workspaces-client-properties
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReconnectEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can cache their credentials on the Amazon WorkSpaces client. When enabled, users can choose to reconnect to their WorkSpaces without re-entering their credentials. \"\n        }\n      ]\n    },\n    \"LogUploadEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogUploadEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can upload diagnostic log files of Amazon WorkSpaces client directly to WorkSpaces to troubleshoot issues when using the WorkSpaces client. When enabled, the log files will be sent to WorkSpaces automatically and will be applied to all users in the specified directory.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes an Amazon WorkSpaces\
  \ client.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-client-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-client-properties-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ClientProperties
---
