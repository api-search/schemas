---
description: Represents the output of a <code>ListApplicationRevisions</code> operation.
layout: schema
name: ListApplicationRevisionsOutput
properties_list:
- description: ''
  name: revisions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-application-revisions-output-schema.json
slug: amazon-codedeploy-list-application-revisions-output
source_filename: amazon-codedeploy-list-application-revisions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-application-revisions-output-schema.json\",\n  \"title\": \"ListApplicationRevisionsOutput\",\n  \"description\": \"Represents the output of a <code>ListApplicationRevisions</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionLocationList\"\n        },\n        {\n          \"description\": \"A list of locations that contain the matching revisions.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent list application\
  \ revisions call to return the next set of application revisions in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-application-revisions-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListApplicationRevisionsOutput
---
