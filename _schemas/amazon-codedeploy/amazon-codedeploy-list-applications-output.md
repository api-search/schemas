---
description: Represents the output of a ListApplications operation.
layout: schema
name: ListApplicationsOutput
properties_list:
- description: ''
  name: applications
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-applications-output-schema.json
slug: amazon-codedeploy-list-applications-output
source_filename: amazon-codedeploy-list-applications-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-applications-output-schema.json\",\n  \"title\": \"ListApplicationsOutput\",\n  \"description\": \"Represents the output of a ListApplications operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationsList\"\n        },\n        {\n          \"description\": \"A list of application names.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If a large amount of information is returned, an identifier is also returned. It can be used in a subsequent list applications call to return the next set of applications in the list.\"\n    \
  \    }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-applications-output-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListApplicationsOutput
---
