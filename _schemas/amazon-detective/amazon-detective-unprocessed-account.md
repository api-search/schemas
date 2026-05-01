---
description: A member account that could not be processed
layout: schema
name: UnprocessedAccount
properties_list:
- description: The AWS account identifier of the member account that was not processed.
  name: AccountId
  type: string
- description: The reason that the member account request could not be processed.
  name: Reason
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-unprocessed-account-schema.json
slug: amazon-detective-unprocessed-account
source_filename: amazon-detective-unprocessed-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-unprocessed-account-schema.json\",\n  \"title\": \"UnprocessedAccount\",\n  \"description\": \"A member account that could not be processed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account identifier of the member account that was not processed.\",\n      \"example\": \"234567890123\"\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason that the member account request could not be processed.\",\n      \"example\": \"Account not found\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-unprocessed-account-schema.json
tags:
- Forensics
- Investigation
- Security
title: UnprocessedAccount
---
