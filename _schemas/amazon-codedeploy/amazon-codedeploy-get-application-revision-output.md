---
description: Represents the output of a <code>GetApplicationRevision</code> operation.
layout: schema
name: GetApplicationRevisionOutput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: revisionInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-get-application-revision-output-schema.json
slug: amazon-codedeploy-get-application-revision-output
source_filename: amazon-codedeploy-get-application-revision-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-revision-output-schema.json\",\n  \"title\": \"GetApplicationRevisionOutput\",\n  \"description\": \"Represents the output of a <code>GetApplicationRevision</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application that corresponds to the revision.\"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocation\"\n        },\n        {\n          \"description\": \"Additional information about the revision, including type and location.\"\n        }\n      ]\n    },\n    \"revisionInfo\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericRevisionInfo\"\n        },\n        {\n          \"description\": \"General information about the revision.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-get-application-revision-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: GetApplicationRevisionOutput
---
