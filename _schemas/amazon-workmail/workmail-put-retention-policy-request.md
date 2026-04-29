---
description: PutRetentionPolicyRequest schema from Amazon WorkMail API
layout: schema
name: PutRetentionPolicyRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
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
schema_file: json-schema/workmail-put-retention-policy-request-schema.json
slug: workmail-put-retention-policy-request
source_filename: workmail-put-retention-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Name\",\n    \"FolderConfigurations\"\n  ],\n  \"title\": \"PutRetentionPolicyRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization ID.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortString\"\n        },\n        {\n          \"description\": \"The retention policy ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortString\"\n        },\n        {\n          \"description\": \"The retention policy name.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDescription\"\n        },\n        {\n     \
  \     \"description\": \"The retention policy description.\"\n        }\n      ]\n    },\n    \"FolderConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FolderConfigurations\"\n        },\n        {\n          \"description\": \"The retention policy folder configurations.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-retention-policy-request-schema.json\",\n  \"description\": \"PutRetentionPolicyRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-retention-policy-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: PutRetentionPolicyRequest
---
