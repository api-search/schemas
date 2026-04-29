---
description: DeleteRetentionPolicyRequest schema from Amazon WorkMail API
layout: schema
name: DeleteRetentionPolicyRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Id
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-retention-policy-request-schema.json
slug: workmail-delete-retention-policy-request
source_filename: workmail-delete-retention-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Id\"\n  ],\n  \"title\": \"DeleteRetentionPolicyRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The organization ID.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShortString\"\n        },\n        {\n          \"description\": \"The retention policy ID.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-retention-policy-request-schema.json\",\n  \"description\": \"DeleteRetentionPolicyRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-retention-policy-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteRetentionPolicyRequest
---
