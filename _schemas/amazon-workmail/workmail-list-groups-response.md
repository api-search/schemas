---
description: ListGroupsResponse schema from Amazon WorkMail API
layout: schema
name: ListGroupsResponse
properties_list:
- description: ''
  name: Groups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-groups-response-schema.json
slug: workmail-list-groups-response
source_filename: workmail-list-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Groups\"\n        },\n        {\n          \"description\": \"The overview of groups for an organization.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. The value is \\\"null\\\" when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListGroupsResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-groups-response-schema.json\",\n  \"description\": \"ListGroupsResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-groups-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListGroupsResponse
---
