---
description: Represents the input of a <code>DeleteApplication</code> operation.
layout: schema
name: DeleteApplicationInput
properties_list:
- description: ''
  name: applicationName
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-delete-application-input-schema.json
slug: amazon-codedeploy-delete-application-input
source_filename: amazon-codedeploy-delete-application-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-application-input-schema.json\",\n  \"title\": \"DeleteApplicationInput\",\n  \"description\": \"Represents the input of a <code>DeleteApplication</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-delete-application-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: DeleteApplicationInput
---
