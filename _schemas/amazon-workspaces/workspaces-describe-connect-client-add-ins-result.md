---
description: DescribeConnectClientAddInsResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeConnectClientAddInsResult
properties_list:
- description: ''
  name: AddIns
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-connect-client-add-ins-result-schema.json
slug: workspaces-describe-connect-client-add-ins-result
source_filename: workspaces-describe-connect-client-add-ins-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddIns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectClientAddInList\"\n        },\n        {\n          \"description\": \"Information about client add-ins.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeConnectClientAddInsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connect-client-add-ins-result-schema.json\",\n  \"description\": \"DescribeConnectClientAddInsResult schema from Amazon WorkSpaces API\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connect-client-add-ins-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeConnectClientAddInsResult
---
