---
description: Information about the instances to be used in the replacement environment in a blue/green deployment.
layout: schema
name: TargetInstances
properties_list:
- description: ''
  name: tagFilters
  type: object
- description: ''
  name: autoScalingGroups
  type: object
- description: ''
  name: ec2TagSet
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-target-instances-schema.json
slug: amazon-codedeploy-target-instances
source_filename: amazon-codedeploy-target-instances-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-target-instances-schema.json\",\n  \"title\": \"TargetInstances\",\n  \"description\": \"Information about the instances to be used in the replacement environment in a blue/green deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tagFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagFilterList\"\n        },\n        {\n          \"description\": \"The tag filter key, type, and value used to identify Amazon EC2 instances in a replacement environment for a blue/green deployment. Cannot be used in the same call as <code>ec2TagSet</code>.\"\n        }\n      ]\n    },\n    \"autoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupNameList\"\n        },\n        {\n     \
  \     \"description\": \"The names of one or more Auto Scaling groups to identify a replacement environment for a blue/green deployment.\"\n        }\n      ]\n    },\n    \"ec2TagSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagSet\"\n        },\n        {\n          \"description\": \"Information about the groups of Amazon EC2 instance tags that an instance must be identified by in order for it to be included in the replacement environment for a blue/green deployment. Cannot be used in the same call as <code>tagFilters</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-target-instances-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TargetInstances
---
