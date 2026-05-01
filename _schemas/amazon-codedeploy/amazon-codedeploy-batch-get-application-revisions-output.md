---
description: Represents the output of a <code>BatchGetApplicationRevisions</code> operation.
layout: schema
name: BatchGetApplicationRevisionsOutput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: revisions
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-application-revisions-output-schema.json
slug: amazon-codedeploy-batch-get-application-revisions-output
source_filename: amazon-codedeploy-batch-get-application-revisions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-application-revisions-output-schema.json\",\n  \"title\": \"BatchGetApplicationRevisionsOutput\",\n  \"description\": \"Represents the output of a <code>BatchGetApplicationRevisions</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application that corresponds to the revisions.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"Information about errors that might have occurred during the API call.\"\n        }\n      ]\n    },\n\
  \    \"revisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionInfoList\"\n        },\n        {\n          \"description\": \"Additional information about the revisions, including the type and location.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-application-revisions-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetApplicationRevisionsOutput
---
