---
description: Describes a WorkSpace.
layout: schema
name: WorkspaceProperties
properties_list:
- description: ''
  name: RunningMode
  type: object
- description: ''
  name: RunningModeAutoStopTimeoutInMinutes
  type: object
- description: ''
  name: RootVolumeSizeGib
  type: object
- description: ''
  name: UserVolumeSizeGib
  type: object
- description: ''
  name: ComputeTypeName
  type: object
- description: ''
  name: Protocols
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-properties-schema.json
slug: workspaces-workspace-properties
source_filename: workspaces-workspace-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunningMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunningMode\"\n        },\n        {\n          \"description\": \"<p>The running mode. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/running-mode.html\\\">Manage the WorkSpace Running Mode</a>.</p> <note> <p>The <code>MANUAL</code> value is only supported by Amazon WorkSpaces Core. Contact your account team to be allow-listed to use this value. For more information, see <a href=\\\"http://aws.amazon.com/workspaces/core/\\\">Amazon WorkSpaces Core</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"RunningModeAutoStopTimeoutInMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunningModeAutoStopTimeoutInMinutes\"\n        },\n        {\n          \"description\": \"The time after a user logs off when WorkSpaces are automatically stopped. Configured\
  \ in 60-minute intervals.\"\n        }\n      ]\n    },\n    \"RootVolumeSizeGib\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RootVolumeSizeGib\"\n        },\n        {\n          \"description\": \"The size of the root volume. For important information about how to modify the size of the root and user volumes, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/modify-workspaces.html\\\">Modify a WorkSpace</a>.\"\n        }\n      ]\n    },\n    \"UserVolumeSizeGib\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserVolumeSizeGib\"\n        },\n        {\n          \"description\": \"The size of the user storage. For important information about how to modify the size of the root and user volumes, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/modify-workspaces.html\\\">Modify a WorkSpace</a>.\"\n        }\n      ]\n    },\n    \"ComputeTypeName\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/Compute\"\n        },\n        {\n          \"description\": \"The compute type. For more information, see <a href=\\\"http://aws.amazon.com/workspaces/details/#Amazon_WorkSpaces_Bundles\\\">Amazon WorkSpaces Bundles</a>.\"\n        }\n      ]\n    },\n    \"Protocols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProtocolList\"\n        },\n        {\n          \"description\": \"<p>The protocol. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/amazon-workspaces-protocols.html\\\"> Protocols for Amazon WorkSpaces</a>.</p> <note> <ul> <li> <p>Only available for WorkSpaces created with PCoIP bundles.</p> </li> <li> <p>The <code>Protocols</code> property is case sensitive. Ensure you use <code>PCOIP</code> or <code>WSP</code>.</p> </li> <li> <p>Unavailable for Windows 7 WorkSpaces and WorkSpaces using GPU-based bundles (Graphics, GraphicsPro, Graphics.g4dn,\
  \ and GraphicsPro.g4dn).</p> </li> </ul> </note>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-properties-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceProperties
---
