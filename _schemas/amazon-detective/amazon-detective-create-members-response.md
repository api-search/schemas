---
description: Response from creating member accounts
layout: schema
name: CreateMembersResponse
properties_list:
- description: The set of member account invitation or enablement requests.
  name: Members
  type: array
- description: The list of accounts for which Detective was unable to process the invitation.
  name: UnprocessedAccounts
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-create-members-response-schema.json
slug: amazon-detective-create-members-response
source_filename: amazon-detective-create-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-create-members-response-schema.json\",\n  \"title\": \"CreateMembersResponse\",\n  \"description\": \"Response from creating member accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Members\": {\n      \"type\": \"array\",\n      \"description\": \"The set of member account invitation or enablement requests.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MemberDetail\"\n      }\n    },\n    \"UnprocessedAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"The list of accounts for which Detective was unable to process the invitation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UnprocessedAccount\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-create-members-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: CreateMembersResponse
---
