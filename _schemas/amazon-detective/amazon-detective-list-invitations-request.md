---
description: Request to list invitations
layout: schema
name: ListInvitationsRequest
properties_list:
- description: The pagination token for the next page of results.
  name: NextToken
  type: string
- description: The maximum number of invitations to return.
  name: MaxResults
  type: integer
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-invitations-request-schema.json
slug: amazon-detective-list-invitations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-invitations-request-schema.json\",\n  \"title\": \"ListInvitationsRequest\",\n  \"description\": \"Request to list invitations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The pagination token for the next page of results.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of invitations to return.\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-invitations-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListInvitationsRequest
---
