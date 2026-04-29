---
description: The device types and operating systems that can be used to access a WorkSpace. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/workspaces-network-requirements.html">Amazon WorkSpaces Client Network Requirements</a>.
layout: schema
name: WorkspaceAccessProperties
properties_list:
- description: ''
  name: DeviceTypeWindows
  type: object
- description: ''
  name: DeviceTypeOsx
  type: object
- description: ''
  name: DeviceTypeWeb
  type: object
- description: ''
  name: DeviceTypeIos
  type: object
- description: ''
  name: DeviceTypeAndroid
  type: object
- description: ''
  name: DeviceTypeChromeOs
  type: object
- description: ''
  name: DeviceTypeZeroClient
  type: object
- description: ''
  name: DeviceTypeLinux
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-access-properties-schema.json
slug: workspaces-workspace-access-properties
source_filename: workspaces-workspace-access-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceTypeWindows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use Windows clients to access their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeOsx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use macOS clients to access their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeWeb\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can access their WorkSpaces through a web browser.\"\n        }\n      ]\n    },\n    \"DeviceTypeIos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\
  \n        },\n        {\n          \"description\": \"Indicates whether users can use iOS devices to access their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeAndroid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use Android and Android-compatible Chrome OS devices to access their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeChromeOs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use Chromebooks to access their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeZeroClient\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use zero client devices to access\
  \ their WorkSpaces.\"\n        }\n      ]\n    },\n    \"DeviceTypeLinux\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPropertyValue\"\n        },\n        {\n          \"description\": \"Indicates whether users can use Linux clients to access their WorkSpaces.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The device types and operating systems that can be used to access a WorkSpace. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/workspaces-network-requirements.html\\\">Amazon WorkSpaces Client Network Requirements</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceAccessProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-access-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-access-properties-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceAccessProperties
---
