---
description: Represents the output of a <code>BatchGetOnPremisesInstances</code> operation.
layout: schema
name: BatchGetOnPremisesInstancesOutput
properties_list:
- description: ''
  name: instanceInfos
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-on-premises-instances-output-schema.json
slug: amazon-codedeploy-batch-get-on-premises-instances-output
source_filename: amazon-codedeploy-batch-get-on-premises-instances-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-on-premises-instances-output-schema.json\",\n  \"title\": \"BatchGetOnPremisesInstancesOutput\",\n  \"description\": \"Represents the output of a <code>BatchGetOnPremisesInstances</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceInfoList\"\n        },\n        {\n          \"description\": \"Information about the on-premises instances.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-on-premises-instances-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetOnPremisesInstancesOutput
---
