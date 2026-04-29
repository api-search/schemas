---
description: Describes a WorkSpace.
layout: schema
name: Workspace
properties_list:
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: BundleId
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ComputerName
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
  name: ModificationStates
  type: object
- description: ''
  name: RelatedWorkspaces
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-schema.json
slug: workspaces-workspace
source_filename: workspaces-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the WorkSpace.\"\n        }\n      ]\n    },\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the Directory Service directory for the WorkSpace.\"\n        }\n      ]\n    },\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The user for the WorkSpace.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddress\"\n        },\n        {\n          \"description\": \"The IP address of the WorkSpace.\"\n        }\n      ]\n    },\n \
  \   \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceState\"\n        },\n        {\n          \"description\": \"<p>The operational state of the WorkSpace.</p> <note> <p>After a WorkSpace is terminated, the <code>TERMINATED</code> state is returned only briefly before the WorkSpace directory metadata is cleaned up, so this state is rarely returned. To confirm that a WorkSpace is terminated, check for the WorkSpace ID by using <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/api/API_DescribeWorkspaces.html\\\"> DescribeWorkSpaces</a>. If the WorkSpace ID isn't returned, then the WorkSpace has been successfully terminated.</p> </note>\"\n        }\n      ]\n    },\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle used to create the WorkSpace.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetId\"\n        },\n        {\n          \"description\": \"The identifier of the subnet for the WorkSpace.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The text of the error message that is returned if the WorkSpace cannot be created.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceErrorCode\"\n        },\n        {\n          \"description\": \"The error code that is returned if the WorkSpace cannot be created.\"\n        }\n      ]\n    },\n    \"ComputerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputerName\"\n        },\n        {\n          \"description\": \"The name of the WorkSpace, as seen by the operating system. The format\
  \ of this name varies. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/launch-workspaces-tutorials.html\\\"> Launch a WorkSpace</a>. \"\n        }\n      ]\n    },\n    \"VolumeEncryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeEncryptionKey\"\n        },\n        {\n          \"description\": \"The ARN of the symmetric KMS key used to encrypt data stored on your WorkSpace. Amazon WorkSpaces does not support asymmetric KMS keys.\"\n        }\n      ]\n    },\n    \"UserVolumeEncryptionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether the data stored on the user volume is encrypted.\"\n        }\n      ]\n    },\n    \"RootVolumeEncryptionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n    \
  \      \"description\": \"Indicates whether the data stored on the root volume is encrypted.\"\n        }\n      ]\n    },\n    \"WorkspaceProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceProperties\"\n        },\n        {\n          \"description\": \"The properties of the WorkSpace.\"\n        }\n      ]\n    },\n    \"ModificationStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModificationStateList\"\n        },\n        {\n          \"description\": \"The modification states of the WorkSpace.\"\n        }\n      ]\n    },\n    \"RelatedWorkspaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedWorkspaces\"\n        },\n        {\n          \"description\": \"The standby WorkSpace or primary WorkSpace related to the specified WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Workspace\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: Workspace
---
