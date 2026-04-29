---
description: GetMasterAccountResponse schema from Amazon Macie API
layout: schema
name: GetMasterAccountResponse
properties_list:
- description: ''
  name: master
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-master-account-response-schema.json
slug: amazon-macie-get-master-account-response
source_filename: amazon-macie-get-master-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-master-account-response-schema.json\",\n  \"title\": \"GetMasterAccountResponse\",\n  \"description\": \"GetMasterAccountResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"master\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Invitation\"\n        },\n        {\n          \"description\": \"(Deprecated) The Amazon Web Services account ID for the administrator account. If the accounts are associated by a Macie membership invitation, this object also provides details about the invitation that was sent to establish the relationship between the accounts.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-master-account-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetMasterAccountResponse
---
