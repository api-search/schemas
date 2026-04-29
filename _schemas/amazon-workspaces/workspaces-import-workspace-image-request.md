---
description: ImportWorkspaceImageRequest schema from Amazon WorkSpaces API
layout: schema
name: ImportWorkspaceImageRequest
properties_list:
- description: ''
  name: Ec2ImageId
  type: object
- description: ''
  name: IngestionProcess
  type: object
- description: ''
  name: ImageName
  type: object
- description: ''
  name: ImageDescription
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Applications
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-import-workspace-image-request-schema.json
slug: workspaces-import-workspace-image-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Ec2ImageId\",\n    \"IngestionProcess\",\n    \"ImageName\",\n    \"ImageDescription\"\n  ],\n  \"title\": \"ImportWorkspaceImageRequest\",\n  \"properties\": {\n    \"Ec2ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2ImageId\"\n        },\n        {\n          \"description\": \"The identifier of the EC2 image.\"\n        }\n      ]\n    },\n    \"IngestionProcess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageIngestionProcess\"\n        },\n        {\n          \"description\": \"<p>The ingestion process to be used when importing the image, depending on which protocol you want to use for your BYOL Workspace image, either PCoIP, WorkSpaces Streaming Protocol (WSP), or bring your own protocol (BYOP). To use WSP, specify a value that ends in <code>_WSP</code>. To use PCoIP, specify a value that does not end in <code>_WSP</code>. To use\
  \ BYOP, specify a value that ends in <code>_BYOP</code>.</p> <p>For non-GPU-enabled bundles (bundles other than Graphics or GraphicsPro), specify <code>BYOL_REGULAR</code>, <code>BYOL_REGULAR_WSP</code>, or <code>BYOL_REGULAR_BYOP</code>, depending on the protocol.</p> <note> <p>The <code>BYOL_REGULAR_BYOP</code> and <code>BYOL_GRAPHICS_G4DN_BYOP</code> values are only supported by Amazon WorkSpaces Core. Contact your account team to be allow-listed to use these values. For more information, see <a href=\\\"http://aws.amazon.com/workspaces/core/\\\">Amazon WorkSpaces Core</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"ImageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageName\"\n        },\n        {\n          \"description\": \"The name of the WorkSpace image.\"\n        }\n      ]\n    },\n    \"ImageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageDescription\"\n      \
  \  },\n        {\n          \"description\": \"The description of the WorkSpace image.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags. Each WorkSpaces resource can have a maximum of 50 tags.\"\n        }\n      ]\n    },\n    \"Applications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationList\"\n        },\n        {\n          \"description\": \"<p>If specified, the version of Microsoft Office to subscribe to. Valid only for Windows 10 and 11 BYOL images. For more information about subscribing to Office for BYOL images, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/byol-windows-images.html\\\"> Bring Your Own Windows Desktop Licenses</a>.</p> <note> <ul> <li> <p>Although this parameter is an array, only one item is allowed at this time.</p> </li> <li> <p>Windows 11 only supports\
  \ <code>Microsoft_Office_2019</code>.</p> </li> </ul> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-workspace-image-request-schema.json\",\n  \"description\": \"ImportWorkspaceImageRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-workspace-image-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ImportWorkspaceImageRequest
---
