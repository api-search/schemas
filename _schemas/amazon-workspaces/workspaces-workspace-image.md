---
description: Describes a WorkSpace image.
layout: schema
name: WorkspaceImage
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
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: OwnerAccountId
  type: object
- description: ''
  name: Updates
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-image-schema.json
slug: workspaces-workspace-image
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the image.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n        },\n        {\n          \"description\": \"The description of the image.\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"The operating system that the image is running. \"\n        }\n      ]\n    },\n\
  \    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageState\"\n        },\n        {\n          \"description\": \"The status of the image.\"\n        }\n      ]\n    },\n    \"RequiredTenancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageRequiredTenancy\"\n        },\n        {\n          \"description\": \"Specifies whether the image is running on dedicated hardware. When Bring Your Own License (BYOL) is enabled, this value is set to <code>DEDICATED</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/byol-windows-images.html\\\">Bring Your Own Windows Desktop Images</a>.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageErrorCode\"\n        },\n        {\n          \"description\": \"The error code that is returned for the image.\"\n        }\n\
  \      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The text of the error message that is returned for the image.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date when the image was created. If the image has been shared, the Amazon Web Services account that the image has been shared with sees the original creation date of the image.\"\n        }\n      ]\n    },\n    \"OwnerAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that owns the image.\"\n        }\n      ]\n    },\n    \"Updates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateResult\"\
  \n        },\n        {\n          \"description\": \"The updates (if any) that are available for the specified image.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a WorkSpace image.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceImage\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-image-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-image-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceImage
---
