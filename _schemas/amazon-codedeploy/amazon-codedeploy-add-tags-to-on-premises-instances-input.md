---
description: Represents the input of, and adds tags to, an on-premises instance operation.
layout: schema
name: AddTagsToOnPremisesInstancesInput
properties_list:
- description: ''
  name: tags
  type: object
- description: ''
  name: instanceNames
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-add-tags-to-on-premises-instances-input-schema.json
slug: amazon-codedeploy-add-tags-to-on-premises-instances-input
source_filename: amazon-codedeploy-add-tags-to-on-premises-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-add-tags-to-on-premises-instances-input-schema.json\",\n  \"title\": \"AddTagsToOnPremisesInstancesInput\",\n  \"description\": \"Represents the input of, and adds tags to, an on-premises instance operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>The tag key-value pairs to add to the on-premises instances.</p> <p>Keys and values are both required. Keys cannot be null or empty strings. Value-only tags are not allowed.</p>\"\n        }\n      ]\n    },\n    \"instanceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceNameList\"\n        },\n        {\n          \"description\"\
  : \"The names of the on-premises instances to which to add tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\",\n    \"instanceNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-add-tags-to-on-premises-instances-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: AddTagsToOnPremisesInstancesInput
---
