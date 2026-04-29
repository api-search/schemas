---
description: ListGroupMembersResponse schema from Amazon WorkMail API
layout: schema
name: ListGroupMembersResponse
properties_list:
- description: ''
  name: Members
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-group-members-response-schema.json
slug: workmail-list-group-members-response
source_filename: workmail-list-group-members-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Members\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Members\"\n        },\n        {\n          \"description\": \"The members associated to the group.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The first call does not contain any tokens.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListGroupMembersResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-group-members-response-schema.json\",\n  \"description\": \"ListGroupMembersResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-group-members-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListGroupMembersResponse
---
