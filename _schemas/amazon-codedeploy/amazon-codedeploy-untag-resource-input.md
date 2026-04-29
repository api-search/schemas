---
description: UntagResourceInput schema from Amazon CodeDeploy
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-untag-resource-input-schema.json
slug: amazon-codedeploy-untag-resource-input
source_filename: amazon-codedeploy-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) that specifies from which resource to disassociate the tags with the keys in the <code>TagKeys</code> input parameter. \"\n        }\n      ]\n    },\n    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \" A list of keys of <code>Tag</code> objects. The <code>Tag</code> objects identified by the keys are\
  \ disassociated from the resource specified by the <code>ResourceArn</code> input parameter. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-untag-resource-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: UntagResourceInput
---
