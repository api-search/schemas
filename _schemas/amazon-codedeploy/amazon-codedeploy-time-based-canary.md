---
description: A configuration that shifts traffic from one version of a Lambda function or Amazon ECS task set to another in two increments. The original and target Lambda function versions or ECS task sets are specified in the deployment's AppSpec file.
layout: schema
name: TimeBasedCanary
properties_list:
- description: ''
  name: canaryPercentage
  type: object
- description: ''
  name: canaryInterval
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-time-based-canary-schema.json
slug: amazon-codedeploy-time-based-canary
source_filename: amazon-codedeploy-time-based-canary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-based-canary-schema.json\",\n  \"title\": \"TimeBasedCanary\",\n  \"description\": \"A configuration that shifts traffic from one version of a Lambda function or Amazon ECS task set to another in two increments. The original and target Lambda function versions or ECS task sets are specified in the deployment's AppSpec file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"canaryPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of traffic to shift in the first increment of a <code>TimeBasedCanary</code> deployment.\"\n        }\n      ]\n    },\n    \"canaryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WaitTimeInMins\"\
  \n        },\n        {\n          \"description\": \"The number of minutes between the first and second traffic shifts of a <code>TimeBasedCanary</code> deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-based-canary-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TimeBasedCanary
---
