---
description: CreateWorkspaceImageResult schema from Amazon WorkSpaces API
layout: schema
name: CreateWorkspaceImageResult
properties_list:
- description: ''
  name: ImageId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: RequiredTenancy
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: OwnerAccountId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-workspace-image-result-schema.json
slug: workspaces-create-workspace-image-result
source_filename: workspaces-create-workspace-image-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the new WorkSpace image.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n        },\n        {\n          \"description\": \"The description of the image.\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"The operating system that the image is running.\"\n        }\n    \
  \  ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageState\"\n        },\n        {\n          \"description\": \"The availability status of the image.\"\n        }\n      ]\n    },\n    \"RequiredTenancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageRequiredTenancy\"\n        },\n        {\n          \"description\": \"Specifies whether the image is running on dedicated hardware. When Bring Your Own License (BYOL) is enabled, this value is set to DEDICATED. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/byol-windows-images.htm\\\"> Bring Your Own Windows Desktop Images.</a>.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the image was created.\"\n        }\n      ]\n   \
  \ },\n    \"OwnerAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that owns the image.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateWorkspaceImageResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-image-result-schema.json\",\n  \"description\": \"CreateWorkspaceImageResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-image-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateWorkspaceImageResult
---
