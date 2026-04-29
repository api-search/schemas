---
description: ListAccessControlRulesResponse schema from Amazon WorkMail API
layout: schema
name: ListAccessControlRulesResponse
properties_list:
- description: ''
  name: Rules
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-access-control-rules-response-schema.json
slug: workmail-list-access-control-rules-response
source_filename: workmail-list-access-control-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRulesList\"\n        },\n        {\n          \"description\": \"The access control rules.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAccessControlRulesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-access-control-rules-response-schema.json\",\n  \"description\": \"ListAccessControlRulesResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-access-control-rules-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListAccessControlRulesResponse
---
