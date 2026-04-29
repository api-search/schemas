---
description: DeleteAccessControlRuleRequest schema from Amazon WorkMail API
layout: schema
name: DeleteAccessControlRuleRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-access-control-rule-request-schema.json
slug: workmail-delete-access-control-rule-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"Name\"\n  ],\n  \"title\": \"DeleteAccessControlRuleRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleName\"\n        },\n        {\n          \"description\": \"The name of the access control rule.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-access-control-rule-request-schema.json\",\n  \"description\": \"DeleteAccessControlRuleRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-access-control-rule-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteAccessControlRuleRequest
---
