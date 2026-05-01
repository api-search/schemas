---
description: A configuration that shifts traffic from one version of a Lambda function or ECS task set to another in equal increments, with an equal number of minutes between each increment. The original and target Lambda function versions or ECS task sets are specified in the deployment's AppSpec file.
layout: schema
name: TimeBasedLinear
properties_list:
- description: ''
  name: linearPercentage
  type: object
- description: ''
  name: linearInterval
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-time-based-linear-schema.json
slug: amazon-codedeploy-time-based-linear
source_filename: amazon-codedeploy-time-based-linear-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-based-linear-schema.json\",\n  \"title\": \"TimeBasedLinear\",\n  \"description\": \"A configuration that shifts traffic from one version of a Lambda function or ECS task set to another in equal increments, with an equal number of minutes between each increment. The original and target Lambda function versions or ECS task sets are specified in the deployment's AppSpec file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"linearPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of traffic that is shifted at the start of each increment of a <code>TimeBasedLinear</code> deployment.\"\n        }\n      ]\n    },\n    \"linearInterval\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/WaitTimeInMins\"\n        },\n        {\n          \"description\": \"The number of minutes between each incremental traffic shift of a <code>TimeBasedLinear</code> deployment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-time-based-linear-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TimeBasedLinear
---
