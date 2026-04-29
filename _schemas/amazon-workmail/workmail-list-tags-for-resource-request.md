---
description: ListTagsForResourceRequest schema from Amazon WorkMail API
layout: schema
name: ListTagsForResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-tags-for-resource-request-schema.json
slug: workmail-list-tags-for-resource-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\"\n  ],\n  \"title\": \"ListTagsForResourceRequest\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The resource ARN.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-tags-for-resource-request-schema.json\",\n  \"description\": \"ListTagsForResourceRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-tags-for-resource-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListTagsForResourceRequest
---
