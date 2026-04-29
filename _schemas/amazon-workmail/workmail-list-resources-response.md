---
description: ListResourcesResponse schema from Amazon WorkMail API
layout: schema
name: ListResourcesResponse
properties_list:
- description: ''
  name: Resources
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-resources-response-schema.json
slug: workmail-list-resources-response
source_filename: workmail-list-resources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resources\"\n        },\n        {\n          \"description\": \"One page of the organization's resource representation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" The token used to paginate through all the organization's resources. While results are still available, it has an associated value. When the last page is reached, the token is empty.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResourcesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-resources-response-schema.json\",\n  \"description\": \"ListResourcesResponse schema\
  \ from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-resources-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListResourcesResponse
---
