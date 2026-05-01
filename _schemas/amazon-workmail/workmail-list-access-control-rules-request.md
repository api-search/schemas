---
description: ListAccessControlRulesRequest schema from Amazon WorkMail API
layout: schema
name: ListAccessControlRulesRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-access-control-rules-request-schema.json
slug: workmail-list-access-control-rules-request
source_filename: workmail-list-access-control-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"ListAccessControlRulesRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-access-control-rules-request-schema.json\",\n  \"description\": \"ListAccessControlRulesRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-access-control-rules-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListAccessControlRulesRequest
---
