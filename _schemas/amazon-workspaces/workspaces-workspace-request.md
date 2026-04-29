---
description: Describes the information used to create a WorkSpace.
layout: schema
name: WorkspaceRequest
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: BundleId
  type: object
- description: ''
  name: VolumeEncryptionKey
  type: object
- description: ''
  name: UserVolumeEncryptionEnabled
  type: object
- description: ''
  name: RootVolumeEncryptionEnabled
  type: object
- description: ''
  name: WorkspaceProperties
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-request-schema.json
slug: workspaces-workspace-request
source_filename: workspaces-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"DirectoryId\",\n    \"UserName\",\n    \"BundleId\"\n  ],\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the Directory Service directory for the WorkSpace. You can use <a>DescribeWorkspaceDirectories</a> to list the available directories.\"\n        }\n      ]\n    },\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The user name of the user for the WorkSpace. This user name must exist in the Directory Service directory for the WorkSpace.\"\n        }\n      ]\n    },\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle for\
  \ the WorkSpace. You can use <a>DescribeWorkspaceBundles</a> to list the available bundles.\"\n        }\n      ]\n    },\n    \"VolumeEncryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeEncryptionKey\"\n        },\n        {\n          \"description\": \"The ARN of the symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.\"\n        }\n      ]\n    },\n    \"UserVolumeEncryptionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether the data stored on the user volume is encrypted.\"\n        }\n      ]\n    },\n    \"RootVolumeEncryptionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether the data stored on the root volume is encrypted.\"\
  \n        }\n      ]\n    },\n    \"WorkspaceProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceProperties\"\n        },\n        {\n          \"description\": \"The WorkSpace properties.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags for the WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the information used to create a WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-request-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceRequest
---
