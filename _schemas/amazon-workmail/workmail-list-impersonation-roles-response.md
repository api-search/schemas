---
description: ListImpersonationRolesResponse schema from Amazon WorkMail API
layout: schema
name: ListImpersonationRolesResponse
properties_list:
- description: ''
  name: Roles
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-impersonation-roles-response-schema.json
slug: workmail-list-impersonation-roles-response
source_filename: workmail-list-impersonation-roles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Roles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleList\"\n        },\n        {\n          \"description\": \"The list of impersonation roles under the given WorkMail organization.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to retrieve the next page of results. The value is <code>null</code> when there are no results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListImpersonationRolesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-impersonation-roles-response-schema.json\",\n  \"description\": \"ListImpersonationRolesResponse schema from Amazon WorkMail\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-impersonation-roles-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListImpersonationRolesResponse
---
