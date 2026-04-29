---
description: Response from deleting member accounts
layout: schema
name: DeleteMembersResponse
properties_list:
- description: The list of AWS account identifiers of the member accounts that Detective successfully deleted.
  name: AccountIds
  type: array
- description: The list of member accounts that Detective was unable to delete.
  name: UnprocessedAccounts
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-delete-members-response-schema.json
slug: amazon-detective-delete-members-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-delete-members-response-schema.json\",\n  \"title\": \"DeleteMembersResponse\",\n  \"description\": \"Response from deleting member accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountIds\": {\n      \"type\": \"array\",\n      \"description\": \"The list of AWS account identifiers of the member accounts that Detective successfully deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"UnprocessedAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"The list of member accounts that Detective was unable to delete.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UnprocessedAccount\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-delete-members-response-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: DeleteMembersResponse
---
