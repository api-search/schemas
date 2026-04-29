---
description: The configuration that specifies how traffic is shifted from one version of a Lambda function to another version during an Lambda deployment, or from one Amazon ECS task set to another during an Amazon ECS deployment.
layout: schema
name: TrafficRoutingConfig
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: timeBasedCanary
  type: object
- description: ''
  name: timeBasedLinear
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-traffic-routing-config-schema.json
slug: amazon-codedeploy-traffic-routing-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-traffic-routing-config-schema.json\",\n  \"title\": \"TrafficRoutingConfig\",\n  \"description\": \"The configuration that specifies how traffic is shifted from one version of a Lambda function to another version during an Lambda deployment, or from one Amazon ECS task set to another during an Amazon ECS deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficRoutingType\"\n        },\n        {\n          \"description\": \"The type of traffic shifting (<code>TimeBasedCanary</code> or <code>TimeBasedLinear</code>) used by a deployment configuration.\"\n        }\n      ]\n    },\n    \"timeBasedCanary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeBasedCanary\"\
  \n        },\n        {\n          \"description\": \"A configuration that shifts traffic from one version of a Lambda function or ECS task set to another in two increments. The original and target Lambda function versions or ECS task sets are specified in the deployment's AppSpec file.\"\n        }\n      ]\n    },\n    \"timeBasedLinear\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeBasedLinear\"\n        },\n        {\n          \"description\": \"A configuration that shifts traffic from one version of a Lambda function or Amazon ECS task set to another in equal increments, with an equal number of minutes between each increment. The original and target Lambda function versions or Amazon ECS task sets are specified in the deployment's AppSpec file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-traffic-routing-config-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TrafficRoutingConfig
---
