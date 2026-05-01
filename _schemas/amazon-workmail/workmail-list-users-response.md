---
description: ListUsersResponse schema from Amazon WorkMail API
layout: schema
name: ListUsersResponse
properties_list:
- description: ''
  name: Users
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-users-response-schema.json
slug: workmail-list-users-response
source_filename: workmail-list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Users\"\n        },\n        {\n          \"description\": \"The overview of users for an organization.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" The token to use to retrieve the next page of results. This value is `null` when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListUsersResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-users-response-schema.json\",\n  \"description\": \"ListUsersResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-users-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListUsersResponse
---
