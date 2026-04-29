---
description: GetDefaultRetentionPolicyResponse schema from Amazon WorkMail API
layout: schema
name: GetDefaultRetentionPolicyResponse
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: FolderConfigurations
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-get-default-retention-policy-response-schema.json
slug: workmail-get-default-retention-policy-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortString\"\n        },\n        {\n          \"description\": \"The retention policy ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortString\"\n        },\n        {\n          \"description\": \"The retention policy name.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The retention policy description.\"\n        }\n      ]\n    },\n    \"FolderConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FolderConfigurations\"\n        },\n        {\n          \"description\": \"The retention policy folder configurations.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"GetDefaultRetentionPolicyResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-default-retention-policy-response-schema.json\",\n  \"description\": \"GetDefaultRetentionPolicyResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-get-default-retention-policy-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: GetDefaultRetentionPolicyResponse
---
