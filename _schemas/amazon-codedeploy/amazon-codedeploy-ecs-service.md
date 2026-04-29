---
description: Contains the service and cluster names used to identify an Amazon ECS deployment's target.
layout: schema
name: ECSService
properties_list:
- description: ''
  name: serviceName
  type: object
- description: ''
  name: clusterName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-ecs-service-schema.json
slug: amazon-codedeploy-ecs-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-service-schema.json\",\n  \"title\": \"ECSService\",\n  \"description\": \" Contains the service and cluster names used to identify an Amazon ECS deployment's target. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceName\"\n        },\n        {\n          \"description\": \" The name of the target Amazon ECS service. \"\n        }\n      ]\n    },\n    \"clusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSClusterName\"\n        },\n        {\n          \"description\": \" The name of the cluster that the Amazon ECS service is associated with. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-service-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ECSService
---
