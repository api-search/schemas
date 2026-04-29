---
description: Represents the input of an <code>UpdateApplication</code> operation.
layout: schema
name: UpdateApplicationInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: newApplicationName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-update-application-input-schema.json
slug: amazon-codedeploy-update-application-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-application-input-schema.json\",\n  \"title\": \"UpdateApplicationInput\",\n  \"description\": \"Represents the input of an <code>UpdateApplication</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The current name of the application you want to change.\"\n        }\n      ]\n    },\n    \"newApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The new name to give the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-update-application-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: UpdateApplicationInput
---
