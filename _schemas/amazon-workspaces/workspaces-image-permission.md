---
description: Describes the Amazon Web Services accounts that have been granted permission to use a shared image. For more information about sharing images, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/share-custom-image.html"> Share or Unshare a Custom WorkSpaces Image</a>.
layout: schema
name: ImagePermission
properties_list:
- description: ''
  name: SharedAccountId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-image-permission-schema.json
slug: workspaces-image-permission
source_filename: workspaces-image-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SharedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n        {\n          \"description\": \"The identifier of the Amazon Web Services account that an image has been shared with.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the Amazon Web Services accounts that have been granted permission to use a shared image. For more information about sharing images, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/share-custom-image.html\\\"> Share or Unshare a Custom WorkSpaces Image</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImagePermission\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-image-permission-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-image-permission-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ImagePermission
---
