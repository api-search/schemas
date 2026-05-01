---
description: Describes a WorkSpace bundle.
layout: schema
name: WorkspaceBundle
properties_list:
- description: ''
  name: BundleId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: ImageId
  type: object
- description: ''
  name: RootStorage
  type: object
- description: ''
  name: UserStorage
  type: object
- description: ''
  name: ComputeType
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: BundleType
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-bundle-schema.json
slug: workspaces-workspace-bundle
source_filename: workspaces-workspace-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the bundle.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleOwner\"\n        },\n        {\n          \"description\": \"The owner of the bundle. This is the account identifier of the owner, or <code>AMAZON</code> if the bundle is provided by Amazon Web Services.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description\
  \ of the bundle.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image that was used to create the bundle.\"\n        }\n      ]\n    },\n    \"RootStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RootStorage\"\n        },\n        {\n          \"description\": \"The size of the root volume.\"\n        }\n      ]\n    },\n    \"UserStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserStorage\"\n        },\n        {\n          \"description\": \"The size of the user volume.\"\n        }\n      ]\n    },\n    \"ComputeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeType\"\n        },\n        {\n          \"description\": \"The compute type of the bundle. For more information, see <a href=\\\"http://aws.amazon.com/workspaces/details/#Amazon_WorkSpaces_Bundles\\\
  \">Amazon WorkSpaces Bundles</a>.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last time that the bundle was updated.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the bundle was created.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceBundleState\"\n        },\n        {\n          \"description\": \"The state of the WorkSpace bundle.\"\n        }\n      ]\n    },\n    \"BundleType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleType\"\n        },\n        {\n          \"description\": \"The type of WorkSpace bundle.\"\n        }\n      ]\n    }\n  },\n\
  \  \"description\": \"Describes a WorkSpace bundle.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceBundle\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-bundle-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-bundle-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceBundle
---
