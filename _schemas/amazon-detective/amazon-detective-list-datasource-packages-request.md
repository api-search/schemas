---
description: Request to list datasource packages
layout: schema
name: ListDatasourcePackagesRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArn
  type: string
- description: For requests to get the next page of results.
  name: NextToken
  type: string
- description: The total number of items to return.
  name: MaxResults
  type: integer
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-datasource-packages-request-schema.json
slug: amazon-detective-list-datasource-packages-request
source_filename: amazon-detective-list-datasource-packages-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-datasource-packages-request-schema.json\",\n  \"title\": \"ListDatasourcePackagesRequest\",\n  \"description\": \"Request to list datasource packages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"For requests to get the next page of results.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of items to return.\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-datasource-packages-request-schema.json
tags:
- Forensics
- Investigation
- Security
title: ListDatasourcePackagesRequest
---
