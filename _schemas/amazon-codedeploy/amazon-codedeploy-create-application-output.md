---
description: Represents the output of a <code>CreateApplication</code> operation.
layout: schema
name: CreateApplicationOutput
properties_list:
- description: ''
  name: applicationId
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-create-application-output-schema.json
slug: amazon-codedeploy-create-application-output
source_filename: amazon-codedeploy-create-application-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-application-output-schema.json\",\n  \"title\": \"CreateApplicationOutput\",\n  \"description\": \"Represents the output of a <code>CreateApplication</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationId\"\n        },\n        {\n          \"description\": \"A unique application ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-create-application-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: CreateApplicationOutput
---
