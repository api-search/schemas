---
description: ListTagsForResourceOutput schema from Amazon CodeDeploy
layout: schema
name: ListTagsForResourceOutput
properties_list:
- description: ''
  name: Tags
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-tags-for-resource-output-schema.json
slug: amazon-codedeploy-list-tags-for-resource-output
source_filename: amazon-codedeploy-list-tags-for-resource-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-tags-for-resource-output-schema.json\",\n  \"title\": \"ListTagsForResourceOutput\",\n  \"description\": \"ListTagsForResourceOutput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" A list of tags returned by <code>ListTagsForResource</code>. The tags are associated with the resource identified by the input <code>ResourceArn</code> parameter. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also\
  \ returned. It can be used in a subsequent list application revisions call to return the next set of application revisions in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-tags-for-resource-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListTagsForResourceOutput
---
