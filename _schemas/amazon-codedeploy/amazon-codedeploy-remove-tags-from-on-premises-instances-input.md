---
description: Represents the input of a <code>RemoveTagsFromOnPremisesInstances</code> operation.
layout: schema
name: RemoveTagsFromOnPremisesInstancesInput
properties_list:
- description: ''
  name: tags
  type: object
- description: ''
  name: instanceNames
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-remove-tags-from-on-premises-instances-input-schema.json
slug: amazon-codedeploy-remove-tags-from-on-premises-instances-input
source_filename: amazon-codedeploy-remove-tags-from-on-premises-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-remove-tags-from-on-premises-instances-input-schema.json\",\n  \"title\": \"RemoveTagsFromOnPremisesInstancesInput\",\n  \"description\": \"Represents the input of a <code>RemoveTagsFromOnPremisesInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tag key-value pairs to remove from the on-premises instances.\"\n        }\n      ]\n    },\n    \"instanceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceNameList\"\n        },\n        {\n          \"description\": \"The names of the on-premises instances from which to remove tags.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"tags\",\n    \"instanceNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-remove-tags-from-on-premises-instances-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RemoveTagsFromOnPremisesInstancesInput
---
