---
description: ListTagsForResourceResponse schema from Amazon WorkMail API
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-list-tags-for-resource-response-schema.json
slug: workmail-list-tags-for-resource-response
source_filename: workmail-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of tag key-value pairs.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-tags-for-resource-response-schema.json\",\n  \"description\": \"ListTagsForResourceResponse schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-list-tags-for-resource-response-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: ListTagsForResourceResponse
---
