---
description: A revision for an Lambda or Amazon ECS deployment that is a YAML-formatted or JSON-formatted string. For Lambda and Amazon ECS deployments, the revision is the same as the AppSpec file. This method replaces the deprecated <code>RawString</code> data type.
layout: schema
name: AppSpecContent
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: sha256
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-app-spec-content-schema.json
slug: amazon-codedeploy-app-spec-content
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-app-spec-content-schema.json\",\n  \"title\": \"AppSpecContent\",\n  \"description\": \" A revision for an Lambda or Amazon ECS deployment that is a YAML-formatted or JSON-formatted string. For Lambda and Amazon ECS deployments, the revision is the same as the AppSpec file. This method replaces the deprecated <code>RawString</code> data type. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawStringContent\"\n        },\n        {\n          \"description\": \"<p> The YAML-formatted or JSON-formatted revision string. </p> <p> For an Lambda deployment, the content includes a Lambda function name, the alias for its original version, and the alias for its replacement version. The deployment\
  \ shifts traffic from the original version of the Lambda function to the replacement version. </p> <p> For an Amazon ECS deployment, the content includes the task name, information about the load balancer that serves traffic to the container, and more. </p> <p> For both types of deployments, the content can specify Lambda functions that run at specified hooks, such as <code>BeforeInstall</code>, during a deployment. </p>\"\n        }\n      ]\n    },\n    \"sha256\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawStringSha256\"\n        },\n        {\n          \"description\": \" The SHA256 hash value of the revision content. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-app-spec-content-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: AppSpecContent
---
