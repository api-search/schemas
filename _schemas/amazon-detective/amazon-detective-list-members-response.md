---
description: Response from listing member accounts
layout: schema
name: ListMembersResponse
properties_list:
- description: The list of member accounts in the behavior graph.
  name: MemberDetails
  type: array
- description: If there are more member accounts remaining in the results, then use this pagination token.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-members-response-schema.json
slug: amazon-detective-list-members-response
source_filename: amazon-detective-list-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-members-response-schema.json\",\n  \"title\": \"ListMembersResponse\",\n  \"description\": \"Response from listing member accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MemberDetails\": {\n      \"type\": \"array\",\n      \"description\": \"The list of member accounts in the behavior graph.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MemberDetail\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are more member accounts remaining in the results, then use this pagination token.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-members-response-schema.json
tags:
- Forensics
- Investigation
- Security
title: ListMembersResponse
---
