---
description: Represents the input of a <code>BatchGetOnPremisesInstances</code> operation.
layout: schema
name: BatchGetOnPremisesInstancesInput
properties_list:
- description: ''
  name: instanceNames
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-on-premises-instances-input-schema.json
slug: amazon-codedeploy-batch-get-on-premises-instances-input
source_filename: amazon-codedeploy-batch-get-on-premises-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-on-premises-instances-input-schema.json\",\n  \"title\": \"BatchGetOnPremisesInstancesInput\",\n  \"description\": \"Represents the input of a <code>BatchGetOnPremisesInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceNameList\"\n        },\n        {\n          \"description\": \"The names of the on-premises instances about which to get information. The maximum number of instance names you can specify is 25.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"instanceNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-on-premises-instances-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetOnPremisesInstancesInput
---
