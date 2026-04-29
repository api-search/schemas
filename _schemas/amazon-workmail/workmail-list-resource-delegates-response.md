---
description: ListResourceDelegatesResponse schema from Amazon WorkMail API
layout: schema
name: ListResourceDelegatesResponse
properties_list:
- description: ''
  name: Delegates
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-resource-delegates-response-schema.json
slug: workmail-list-resource-delegates-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Delegates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDelegates\"\n        },\n        {\n          \"description\": \"One page of the resource's delegates.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token used to paginate through the delegates associated with a resource. While results are still available, it has an associated value. When the last page is reached, the token is empty.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResourceDelegatesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-resource-delegates-response-schema.json\",\n  \"description\": \"ListResourceDelegatesResponse\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-resource-delegates-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListResourceDelegatesResponse
---
