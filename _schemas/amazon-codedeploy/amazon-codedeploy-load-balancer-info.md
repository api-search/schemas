---
description: Information about the Elastic Load Balancing load balancer or target group used in a deployment.
layout: schema
name: LoadBalancerInfo
properties_list:
- description: ''
  name: elbInfoList
  type: object
- description: ''
  name: targetGroupInfoList
  type: object
- description: ''
  name: targetGroupPairInfoList
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-load-balancer-info-schema.json
slug: amazon-codedeploy-load-balancer-info
source_filename: amazon-codedeploy-load-balancer-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-load-balancer-info-schema.json\",\n  \"title\": \"LoadBalancerInfo\",\n  \"description\": \"Information about the Elastic Load Balancing load balancer or target group used in a deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elbInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ELBInfoList\"\n        },\n        {\n          \"description\": \"<p>An array that contains information about the load balancer to use for load balancing in a deployment. In Elastic Load Balancing, load balancers are used with Classic Load Balancers.</p> <note> <p> Adding more than one load balancer to the array is not supported. </p> </note>\"\n        }\n      ]\n    },\n    \"targetGroupInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/TargetGroupInfoList\"\n        },\n        {\n          \"description\": \"<p>An array that contains information about the target group to use for load balancing in a deployment. In Elastic Load Balancing, target groups are used with Application Load Balancers.</p> <note> <p> Adding more than one target group to the array is not supported. </p> </note>\"\n        }\n      ]\n    },\n    \"targetGroupPairInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetGroupPairInfoList\"\n        },\n        {\n          \"description\": \" The target group pair information. This is an array of <code>TargeGroupPairInfo</code> objects with a maximum size of one. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-load-balancer-info-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: LoadBalancerInfo
---
