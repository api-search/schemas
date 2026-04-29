---
description: Describes the self-service permissions for a directory. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/enable-user-self-service-workspace-management.html">Enable Self-Service WorkSpace Management Capabilities for Your Users</a>.
layout: schema
name: SelfservicePermissions
properties_list:
- description: ''
  name: RestartWorkspace
  type: object
- description: ''
  name: IncreaseVolumeSize
  type: object
- description: ''
  name: ChangeComputeType
  type: object
- description: ''
  name: SwitchRunningMode
  type: object
- description: ''
  name: RebuildWorkspace
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-selfservice-permissions-schema.json
slug: workspaces-selfservice-permissions
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RestartWorkspace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can restart their WorkSpace.\"\n        }\n      ]\n    },\n    \"IncreaseVolumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can increase the volume size of the drives on their WorkSpace.\"\n        }\n      ]\n    },\n    \"ChangeComputeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can change the compute type (bundle) for their WorkSpace.\"\n        }\n      ]\n    },\n    \"SwitchRunningMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\
  \n        },\n        {\n          \"description\": \"Specifies whether users can switch the running mode of their WorkSpace.\"\n        }\n      ]\n    },\n    \"RebuildWorkspace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReconnectEnum\"\n        },\n        {\n          \"description\": \"Specifies whether users can rebuild the operating system of a WorkSpace to its original state.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the self-service permissions for a directory. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/enable-user-self-service-workspace-management.html\\\">Enable Self-Service WorkSpace Management Capabilities for Your Users</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelfservicePermissions\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-selfservice-permissions-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-selfservice-permissions-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: SelfservicePermissions
---
