---
description: An AWS account to invite to become a member account in a behavior graph
layout: schema
name: Account
properties_list:
- description: The account identifier of the AWS account.
  name: AccountId
  type: string
- description: The AWS account root user email address for the AWS account.
  name: EmailAddress
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-account-schema.json
slug: amazon-detective-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"An AWS account to invite to become a member account in a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account identifier of the AWS account.\",\n      \"example\": \"234567890123\"\n    },\n    \"EmailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account root user email address for the AWS account.\",\n      \"example\": \"security@example.com\"\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"EmailAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-account-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: Account
---
