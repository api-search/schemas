---
description: ListAliasesResponse schema from Amazon WorkMail API
layout: schema
name: ListAliasesResponse
properties_list:
- description: ''
  name: Aliases
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-aliases-response-schema.json
slug: workmail-list-aliases-response
source_filename: workmail-list-aliases-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Aliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Aliases\"\n        },\n        {\n          \"description\": \"The entity's paginated aliases.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value is \\\"null\\\" when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAliasesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-aliases-response-schema.json\",\n  \"description\": \"ListAliasesResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-aliases-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListAliasesResponse
---
