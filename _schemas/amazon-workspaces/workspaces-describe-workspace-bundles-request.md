---
description: DescribeWorkspaceBundlesRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceBundlesRequest
properties_list:
- description: ''
  name: BundleIds
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-bundles-request-schema.json
slug: workspaces-describe-workspace-bundles-request
source_filename: workspaces-describe-workspace-bundles-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeWorkspaceBundlesRequest\",\n  \"properties\": {\n    \"BundleIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleIdList\"\n        },\n        {\n          \"description\": \"The identifiers of the bundles. You cannot combine this parameter with any other filter.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleOwner\"\n        },\n        {\n          \"description\": \"<p>The owner of the bundles. You cannot combine this parameter with any other filter.</p> <p>To describe the bundles provided by Amazon Web Services, specify <code>AMAZON</code>. To describe the bundles that belong to your account, don't specify a value.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\"\
  : \"The token for the next set of results. (You received this token from a previous call.)\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-bundles-request-schema.json\",\n  \"description\": \"DescribeWorkspaceBundlesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-bundles-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceBundlesRequest
---
