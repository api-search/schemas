---
description: GetAdministratorAccountResponse schema from Amazon Macie API
layout: schema
name: GetAdministratorAccountResponse
properties_list:
- description: ''
  name: administrator
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-administrator-account-response-schema.json
slug: amazon-macie-get-administrator-account-response
source_filename: amazon-macie-get-administrator-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-administrator-account-response-schema.json\",\n  \"title\": \"GetAdministratorAccountResponse\",\n  \"description\": \"GetAdministratorAccountResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"administrator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Invitation\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the administrator account. If the accounts are associated by an Amazon Macie membership invitation, this object also provides details about the invitation that was sent to establish the relationship between the accounts.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-administrator-account-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetAdministratorAccountResponse
---
