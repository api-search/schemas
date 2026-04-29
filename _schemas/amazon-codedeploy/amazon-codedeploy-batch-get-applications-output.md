---
description: Represents the output of a <code>BatchGetApplications</code> operation.
layout: schema
name: BatchGetApplicationsOutput
properties_list:
- description: ''
  name: applicationsInfo
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-batch-get-applications-output-schema.json
slug: amazon-codedeploy-batch-get-applications-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-applications-output-schema.json\",\n  \"title\": \"BatchGetApplicationsOutput\",\n  \"description\": \"Represents the output of a <code>BatchGetApplications</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationsInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationsInfoList\"\n        },\n        {\n          \"description\": \"Information about the applications.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-batch-get-applications-output-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: BatchGetApplicationsOutput
---
