---
description: DescribeAccountModificationsRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeAccountModificationsRequest
properties_list:
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-account-modifications-request-schema.json
slug: workspaces-describe-account-modifications-request
source_filename: workspaces-describe-account-modifications-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeAccountModificationsRequest\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-account-modifications-request-schema.json\",\n  \"description\": \"DescribeAccountModificationsRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-account-modifications-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeAccountModificationsRequest
---
