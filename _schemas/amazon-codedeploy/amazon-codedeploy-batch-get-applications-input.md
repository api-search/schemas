---
description: Represents the input of a <code>BatchGetApplications</code> operation.
layout: schema
name: BatchGetApplicationsInput
properties_list:
- description: ''
  name: applicationNames
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-applications-input-schema.json
slug: amazon-codedeploy-batch-get-applications-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-applications-input-schema.json\",\n  \"title\": \"BatchGetApplicationsInput\",\n  \"description\": \"Represents the input of a <code>BatchGetApplications</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationsList\"\n        },\n        {\n          \"description\": \"A list of application names separated by spaces. The maximum number of application names you can specify is 100.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-applications-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetApplicationsInput
---
