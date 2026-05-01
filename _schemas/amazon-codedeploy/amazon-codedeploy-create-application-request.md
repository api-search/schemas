---
description: CreateApplicationRequest schema from Amazon CodeDeploy
layout: schema
name: CreateApplicationRequest
properties_list:
- description: The name of the application.
  name: applicationName
  type: string
- description: The destination platform type for the deployment.
  name: computePlatform
  type: string
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-application-request-schema.json
slug: amazon-codedeploy-create-application-request
source_filename: amazon-codedeploy-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"CreateApplicationRequest schema from Amazon CodeDeploy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"computePlatform\": {\n      \"type\": \"string\",\n      \"description\": \"The destination platform type for the deployment.\",\n      \"enum\": [\n        \"Server\",\n        \"Lambda\",\n        \"ECS\"\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-application-request-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateApplicationRequest
---
