---
description: Represents the input of a RegisterApplicationRevision operation.
layout: schema
name: RegisterApplicationRevisionInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: revision
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-register-application-revision-input-schema.json
slug: amazon-codedeploy-register-application-revision-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-register-application-revision-input-schema.json\",\n  \"title\": \"RegisterApplicationRevisionInput\",\n  \"description\": \"Represents the input of a RegisterApplicationRevision operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A comment about the revision.\"\n        }\n      ]\n    },\n    \"revision\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about the application revision to register, including type and location.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"revision\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-register-application-revision-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RegisterApplicationRevisionInput
---
