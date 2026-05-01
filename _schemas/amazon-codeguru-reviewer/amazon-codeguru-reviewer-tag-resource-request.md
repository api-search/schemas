---
description: TagResourceRequest schema from Amazon CodeGuru Reviewer
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-tag-resource-request-schema.json
slug: amazon-codeguru-reviewer-tag-resource-request
source_filename: amazon-codeguru-reviewer-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>An array of key-value pairs used to tag an associated repository. A tag is a custom attribute label with two parts:</p> <ul> <li> <p>A <i>tag key</i> (for example, <code>CostCenter</code>, <code>Environment</code>, <code>Project</code>, or <code>Secret</code>). Tag keys are case sensitive.</p> </li> <li> <p>An optional field known as a <i>tag value</i> (for example, <code>111122223333</code>, <code>Production</code>,\
  \ or a team name). Omitting the tag value is the same as using an empty string. Like tag keys, tag values are case sensitive.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-tag-resource-request-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: TagResourceRequest
---
