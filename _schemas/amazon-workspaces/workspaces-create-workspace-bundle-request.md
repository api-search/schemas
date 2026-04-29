---
description: CreateWorkspaceBundleRequest schema from Amazon WorkSpaces API
layout: schema
name: CreateWorkspaceBundleRequest
properties_list:
- description: ''
  name: BundleName
  type: object
- description: ''
  name: BundleDescription
  type: object
- description: ''
  name: ImageId
  type: object
- description: ''
  name: ComputeType
  type: object
- description: ''
  name: UserStorage
  type: object
- description: ''
  name: RootStorage
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-workspace-bundle-request-schema.json
slug: workspaces-create-workspace-bundle-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"BundleName\",\n    \"BundleDescription\",\n    \"ImageId\",\n    \"ComputeType\",\n    \"UserStorage\"\n  ],\n  \"title\": \"CreateWorkspaceBundleRequest\",\n  \"properties\": {\n    \"BundleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceBundleName\"\n        },\n        {\n          \"description\": \"The name of the bundle.\"\n        }\n      ]\n    },\n    \"BundleDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceBundleDescription\"\n        },\n        {\n          \"description\": \"The description of the bundle.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image that is used to create the bundle.\"\n        }\n      ]\n    },\n    \"ComputeType\":\
  \ {\n      \"$ref\": \"#/components/schemas/ComputeType\"\n    },\n    \"UserStorage\": {\n      \"$ref\": \"#/components/schemas/UserStorage\"\n    },\n    \"RootStorage\": {\n      \"$ref\": \"#/components/schemas/RootStorage\"\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>The tags associated with the bundle.</p> <note> <p>To add tags at the same time when you're creating the bundle, you must create an IAM policy that grants your IAM user permissions to use <code>workspaces:CreateTags</code>. </p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-bundle-request-schema.json\",\n  \"description\": \"CreateWorkspaceBundleRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspace-bundle-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateWorkspaceBundleRequest
---
