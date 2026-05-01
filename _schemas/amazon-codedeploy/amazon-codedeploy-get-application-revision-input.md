---
description: Represents the input of a <code>GetApplicationRevision</code> operation.
layout: schema
name: GetApplicationRevisionInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: revision
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-application-revision-input-schema.json
slug: amazon-codedeploy-get-application-revision-input
source_filename: amazon-codedeploy-get-application-revision-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-revision-input-schema.json\",\n  \"title\": \"GetApplicationRevisionInput\",\n  \"description\": \"Represents the input of a <code>GetApplicationRevision</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application that corresponds to the revision.\"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Information about the application revision to get, including type and location.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"applicationName\",\n    \"revision\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-revision-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetApplicationRevisionInput
---
