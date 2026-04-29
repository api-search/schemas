---
description: Response from listing invitations
layout: schema
name: ListInvitationsResponse
properties_list:
- description: The list of behavior graphs for which the member account has open or accepted invitations.
  name: Invitations
  type: array
- description: If there are more invitations remaining in the results, then use this pagination token.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-invitations-response-schema.json
slug: amazon-detective-list-invitations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-invitations-response-schema.json\",\n  \"title\": \"ListInvitationsResponse\",\n  \"description\": \"Response from listing invitations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Invitations\": {\n      \"type\": \"array\",\n      \"description\": \"The list of behavior graphs for which the member account has open or accepted invitations.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MemberDetail\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are more invitations remaining in the results, then use this pagination token.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-invitations-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListInvitationsResponse
---
