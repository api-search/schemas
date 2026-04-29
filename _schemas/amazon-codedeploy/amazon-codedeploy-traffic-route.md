---
description: Information about a listener. The listener contains the path used to route traffic that is received from the load balancer to a target group.
layout: schema
name: TrafficRoute
properties_list:
- description: ''
  name: listenerArns
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-traffic-route-schema.json
slug: amazon-codedeploy-traffic-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-traffic-route-schema.json\",\n  \"title\": \"TrafficRoute\",\n  \"description\": \" Information about a listener. The listener contains the path used to route traffic that is received from the load balancer to a target group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"listenerArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerArnList\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of one listener. The listener identifies the route between a target group and a load balancer. This is an array of strings with a maximum size of one. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-traffic-route-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TrafficRoute
---
