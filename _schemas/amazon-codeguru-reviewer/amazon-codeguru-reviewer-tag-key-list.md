---
description: TagKeyList schema from Amazon CodeGuru Reviewer
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-tag-key-list-schema.json
slug: amazon-codeguru-reviewer-tag-key-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-tag-key-list-schema.json\",\n  \"title\": \"TagKeyList\",\n  \"description\": \"TagKeyList schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/TagKey\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-tag-key-list-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: TagKeyList
---
