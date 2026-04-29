---
description: Response from getting member details
layout: schema
name: GetMembersResponse
properties_list:
- description: The member account details that Detective retrieved.
  name: MemberDetails
  type: array
- description: The requested member accounts for which Detective was unable to return member details.
  name: UnprocessedAccounts
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-get-members-response-schema.json
slug: amazon-detective-get-members-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-members-response-schema.json\",\n  \"title\": \"GetMembersResponse\",\n  \"description\": \"Response from getting member details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MemberDetails\": {\n      \"type\": \"array\",\n      \"description\": \"The member account details that Detective retrieved.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MemberDetail\"\n      }\n    },\n    \"UnprocessedAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"The requested member accounts for which Detective was unable to return member details.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UnprocessedAccount\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-get-members-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: GetMembersResponse
---
