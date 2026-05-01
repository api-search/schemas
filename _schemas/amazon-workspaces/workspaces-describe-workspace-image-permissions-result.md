---
description: DescribeWorkspaceImagePermissionsResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceImagePermissionsResult
properties_list:
- description: ''
  name: ImageId
  type: object
- description: ''
  name: ImagePermissions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-image-permissions-result-schema.json
slug: workspaces-describe-workspace-image-permissions-result
source_filename: workspaces-describe-workspace-image-permissions-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceImageId\"\n        },\n        {\n          \"description\": \"The identifier of the image.\"\n        }\n      ]\n    },\n    \"ImagePermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePermissions\"\n        },\n        {\n          \"description\": \"The identifiers of the Amazon Web Services accounts that the image has been shared with.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeWorkspaceImagePermissionsResult\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-image-permissions-result-schema.json\",\n  \"description\": \"DescribeWorkspaceImagePermissionsResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-image-permissions-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceImagePermissionsResult
---
