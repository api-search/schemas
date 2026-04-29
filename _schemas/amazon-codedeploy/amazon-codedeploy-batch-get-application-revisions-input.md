---
description: Represents the input of a <code>BatchGetApplicationRevisions</code> operation.
layout: schema
name: BatchGetApplicationRevisionsInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: revisions
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-application-revisions-input-schema.json
slug: amazon-codedeploy-batch-get-application-revisions-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-application-revisions-input-schema.json\",\n  \"title\": \"BatchGetApplicationRevisionsInput\",\n  \"description\": \"Represents the input of a <code>BatchGetApplicationRevisions</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of an CodeDeploy application about which to get revision information.\"\n        }\n      ]\n    },\n    \"revisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocationList\"\n        },\n        {\n          \"description\": \"An array of <code>RevisionLocation</code> objects that specify information to get\
  \ about the application revisions, including type and location. The maximum number of <code>RevisionLocation</code> objects you can specify is 25.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"revisions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-application-revisions-input-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetApplicationRevisionsInput
---
