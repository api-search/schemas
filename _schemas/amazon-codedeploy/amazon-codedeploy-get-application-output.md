---
description: Represents the output of a <code>GetApplication</code> operation.
layout: schema
name: GetApplicationOutput
properties_list:
- description: ''
  name: application
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-application-output-schema.json
slug: amazon-codedeploy-get-application-output
source_filename: amazon-codedeploy-get-application-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-output-schema.json\",\n  \"title\": \"GetApplicationOutput\",\n  \"description\": \"Represents the output of a <code>GetApplication</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInfo\"\n        },\n        {\n          \"description\": \"Information about the application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetApplicationOutput
---
