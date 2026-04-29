---
description: Request to list member accounts
layout: schema
name: ListMembersRequest
properties_list:
- description: The ARN of the behavior graph to list member accounts for.
  name: GraphArn
  type: string
- description: For requests to retrieve the next page of member account results.
  name: NextToken
  type: string
- description: The maximum number of member accounts to include in the response.
  name: MaxResults
  type: integer
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-members-request-schema.json
slug: amazon-detective-list-members-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-members-request-schema.json\",\n  \"title\": \"ListMembersRequest\",\n  \"description\": \"Request to list member accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph to list member accounts for.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"For requests to retrieve the next page of member account results.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of member accounts to include in the response.\",\n      \"example\": 100\n    }\n  },\n  \"required\"\
  : [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-members-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListMembersRequest
---
