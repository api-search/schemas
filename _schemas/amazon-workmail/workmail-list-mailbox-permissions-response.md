---
description: ListMailboxPermissionsResponse schema from Amazon WorkMail API
layout: schema
name: ListMailboxPermissionsResponse
properties_list:
- description: ''
  name: Permissions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-mailbox-permissions-response-schema.json
slug: workmail-list-mailbox-permissions-response
source_filename: workmail-list-mailbox-permissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Permissions\"\n        },\n        {\n          \"description\": \"One page of the user, group, or resource mailbox permissions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value is \\\"null\\\" when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMailboxPermissionsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mailbox-permissions-response-schema.json\",\n  \"description\": \"ListMailboxPermissionsResponse schema from Amazon WorkMail\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-mailbox-permissions-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListMailboxPermissionsResponse
---
