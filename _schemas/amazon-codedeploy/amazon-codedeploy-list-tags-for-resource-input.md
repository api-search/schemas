---
description: ListTagsForResourceInput schema from Amazon CodeDeploy
layout: schema
name: ListTagsForResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-tags-for-resource-input-schema.json
slug: amazon-codedeploy-list-tags-for-resource-input
source_filename: amazon-codedeploy-list-tags-for-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-tags-for-resource-input-schema.json\",\n  \"title\": \"ListTagsForResourceInput\",\n  \"description\": \"ListTagsForResourceInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The ARN of a CodeDeploy resource. <code>ListTagsForResource</code> returns all the tags associated with the resource that is identified by the <code>ResourceArn</code>. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier returned from the previous <code>ListTagsForResource</code>\
  \ call. It can be used to return the next set of applications in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-tags-for-resource-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListTagsForResourceInput
---
